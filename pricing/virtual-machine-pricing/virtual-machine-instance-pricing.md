# Virtual Machine Instance Pricing

## **Pricing Item**

The price of a virtual machine instance (VM instance) includes CPU, memory, bandwidth cap, system disk, and optional data disk.

### **CPU & Memory**

The detailed specifications of CPU and memory that you are able to select are shown in the following table. The price varies with different specifications and locations and you will see the price when placing the order on zenConsole.

| Instance Model    | vCPU (Core) | RAM (GB) | Bandwidth Cap |
| ----------------- | ----------- | -------- | ------------- |
| Compute Optimized | 1           | 2        | 0.5           |
| Compute Optimized | 2           | 4        | 1             |
| Compute Optimized | 4           | 8        | 1.5           |
| Compute Optimized | 8           | 16       | 2             |
| Compute Optimized | 12          | 24       | 2.5           |
| Compute Optimized | 16          | 32       | 3             |
| Compute Optimized | 24          | 48       | 4.5           |
| Compute Optimized | 32          | 64       | 6             |
| Compute Optimized | 64          | 128      | 6             |
| General Purpose   | 2           | 8        | 1             |
| General Purpose   | 4           | 16       | 1.5           |
| General Purpose   | 8           | 32       | 2             |
| General Purpose   | 16          | 64       | 3             |
| General Purpose   | 24          | 96       | 4.5           |
| General Purpose   | 32          | 128      | 6             |
| Memory Optimized  | 2           | 16       | 1             |
| Memory Optimized  | 4           | 32       | 1.5           |
| Memory Optimized  | 8           | 64       | 2             |
| Memory Optimized  | 16          | 128      | 3             |

### **Bandwidth Cap**

Bandwidth cap refers to the maximum connectivity rate between your VM instance and public network. The price varies according to the size of bandwidth cap and the location of the VM instance. You will see the price when placing the order on zenConsole.

### **System Disk**

System disk is the storage of VM instance’s operating system. The price varies according to the storage volume and the location of the VM instance. You will see the price when placing the order on zenConsole.

### **Data Disk (Optional)**

Data disk provides storage to your business data and data disk uses cloud disk. The price varies according to the storage volume and the location of the VM instance. You will see the price when placing the order on zenConsole.

****

## **Billing Method**

Virtual machine instance is subscribed on a 30-day basis and renewed automatically.

## **Unsubscription**

If you will no longer use the virtual machine instance, you can go to **Billing** > **Subscriptions** > **Auto Renewal**. Find your virtual machine instance and click **Unsubscribe**.

Before the subscription cycle expires, you can click **Resubscribe** to recover the subscription.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">Virtual Machine Instance doesn’t support refund on the unused part if unsubscribed before the subscription cycle expires.</mark>
* <mark style="color:blue;">After being unsubscribed, the instance can be still used till the end of the present subscription cycle.</mark>
{% endhint %}



## FAQ

### **What happens when you no longer have sufficient balance to continue a virtual machine instance?**

When your virtual machine instance fails to renew due to insufficient balance, the following process will ensue:

#### **1. Protection Stage** (24 hours after the renewal failed)

* Your instance will continue to run normally, but you may not create any new instance.
* A reminder email will be sent to users with AdministratorAccess and finance roles to refill account balance in order to continue use.

#### **2. Suspension Stage** (72 hours after the protection stage)

* The instance in service will be suspended, and a suspension notice email will be sent to users with AdministratorAccess and finance roles.
* During this grace period, we will still retain your instance resources and data. After your account balance is refilled, zenConsole will renew the subscription automatically as soon as the suspension stage expires, and you will need to manually power on the instance.

#### **3. Recycle Stage** (once the suspension stage expires)

* Your instance resources will be destroyed and recycled, and you will not be able to recover your data.
* A final notice email will be sent to users with AdministratorAccess and finance roles.

