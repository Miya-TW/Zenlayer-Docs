---
description: >-
  On the left menu bar, go to Compute > Virtual Machine > Virtual Elastic Disk
  to view basic information about the system disk and data disk.
---

# Manage Data Disks

## Prerequisites

After you attach a data disk to a virtual machine instance, you must create and mount one or more file systems on the disk before using it.&#x20;

You have different ways to partition and format a new data disk on a Linux instance and a Windows instance.



## Background Information

Data disks support the GUID Partition Table (GPT) and Master Boot Record (MBR) partition formats.

* GPT: recognize partitions larger than 2 TiB in size and allows an unlimited number of partitions (for Linux)/up to 128 partitions (for Windows) to be created on each disk.
* MBR: recognize partitions up to 2 TiB in size and allows up to four partitions to be created on each disk.



## **Precautions**

* Disk partitioning and formatting are high-risk operations. Proceed with caution when you partition and format disks. This topic applies only to new data disks.
* Only data disks can be partitioned. Please do not partition a system disk, otherwise risks such as system failures and data loss may occur.



## Procedures

### **Linux**

#### Step 1 - Use your password to connect to the instance.&#x20;

Run the following command to view the information of the data disk attached.

```
fdisk -l
```



#### Step 2 - Create a partition for the data disk

**Create a GPT partition**

1\. Run the following command to install Parted and e2fsprogs.

* Install Parted

```
yum install -y parted
```

* Install e2fsprogs

```
yum install -y e2fsprogs
```



2\. Use Parted to partition the data disk. _**/dev/vdb**_ is the disk name for illustration.

&#x20;   1\) Run the following command to start partitioning the data disk.

```
parted /dev/vdb
```

&#x20;   2\) Run the following command to set the partition format to GPT.

```
mklabel gpt
```

&#x20;   3\) Run the following command to create a primary partition and specify the start and end sectors for the partition.

```
mkpart primary 1 100%
```

&#x20;   4\) Run the following command to check whether the partition is aligned.

```
align-check optimal 1
```

&#x20;   5\) Run the following command to view the partition table.

```
print
```

&#x20;   6\) Run the following command to exit Parted.

```
quit
```



3\. Run the following command to re-read the partition table.

```
partprobe
```



4\. Run the following command to view the new partition.

```
fdisk -lu /dev/vdb
```

__

**Create an MBR partition**

MBR partition does not support data disks larger than 2 TiB. If your data disk is larger than 2 TiB in size or may need to be extended to larger than 2 TiB, we recommend that you use the GPT partition format. See [**Create a GPT Partition**](manage-data-disks.md#step-2-create-a-partition-for-the-data-disk) for more details.\


1\. Partition the data disk. _**/dev/vdb**_ is the disk name for illustration.

&#x20;   1\) Run the following command to partition the data disk.

```
fdisk -u /dev/vdb
```

&#x20;   2\) Enter **P** to view the partition information of the data disk.

&#x20;   3\) Enter **N** to create a partition.

&#x20;   4\) Enter **P** to set the partition as a primary partition.

&#x20;   5\) Enter the partition number and press the **Enter** key.

&#x20;   6\) Enter the number of the first available sector and press the **Enter** key.

&#x20;   7\) Enter the number of the last sector and press the **Enter** key.

&#x20;   8\) Enter **P** to view the partition information of the data disk.

&#x20;   9\) Enter **W** to start partitioning. Then, exit after the disk is partitioned.



2\. Run the following command to view the new partition.

```
fdisk -lu /dev/vdb
```



3\. Create a file system for the partition

* Run the following command to create an ext4 file system.

```
mkfs -t ext4 /dev/vdb1
```

* ​​​​​​Run the following command to create an xfs file system.

```
mkfs -t xfs /dev/vdb1
```



4\. Configure the /etc/fstab file and mount the partition

Write the information of the new partition to /etc/fstab to enable this partition to be automatically mounted on instance startup.

&#x20;   1\) Run the following command to back up etc/fstab.

```
cp /etc/fstab /etc/fstab.bak
```

&#x20;   2\) Write the information of the new partition to /etc/fstab.

```
echo `blkid /dev/vdb1 | awk '{print $2}' | sed 's/\"//g'` /mnt ext4 defaults 0 0 >> /etc/fstab
```

&#x20;    Description of the parameters in this command:

* /dev/vdb1: the data disk partition that has a file system created. Replace it with your actual partition name.
* /mnt: the directory to which the partition is mounted. Replace it with the actual directory of your partition.
* ext4: the file system type of the partition. Replace it with the type of the created file system.

&#x20;   3\) Run the following command to check the information of the new partition in /etc/fstab.

```
cat /etc/fstab
```

&#x20;   4\) Run the following command to mount the file system configured in the /etc/fstab file.

```
mount -a
```

&#x20;   5\) Run the following command to check the mount result.

```
df -h
```



### **Windows**

#### Step 1 - Open the **Disk Management** window and find a data disk that is not partitioned or formatted

1. Use your password to connect to the instance.
2. On the Windows Server desktop, click the **Server Manager** icon in the lower-left corner.
3. In the **Server Manager** window, choose **Tools** > **Computer Management** in the upper-right corner.
4. In the left-side navigation pane, choose **Computer Management (Local)** > **Storage** > **Disk Management**.
5. Find a data disk that is not partitioned or formatted, which is in the **Offline** state.

#### Step 2 - Right-click the blank area around the disk and select **Online**

When the disk goes online, it enters the **Not Initialized** state.

#### Step 3 - Right-click the blank area around the disk and select **Initialize Disk**

#### Step 4 - In the **Initialize Disk** dialog box, select the disk, select a partition format, and then click **OK**

#### Step 5 - Right-click the Unallocated section and select **New Simple Volume**

#### Step 6 - In the **New Simple Volume Wizard** dialog box, perform the following operations

1. Click **Next**.
2. In the **Specify Volume Size** step, set **Simple volume size in MB** and click **Next**.
3. In the **Assign Drive Letter or Path** step, select **Assign the following drive letter**, select a drive letter, and then click **Next**.
4. In the **Format Partition** step, select **Format this volume with the following settings**, configure formatting settings, and then click **Next**.
5. Check the settings and click **Finish**.

