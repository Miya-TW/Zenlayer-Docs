# Create a Bare Metal Instance

## **Step 1 - Sign in to zenConsole**

1. Use your email address and password to sign in to [**zenConsole**](https://console.zenlayer.com/dashboard).
2. On the left navigation panel, go to **Compute** > **Bare Metal** > **Bare Metal Instance** > **Create Bare Metal Instance**.

## **Step 2 - Configure basic information for your instance**

{% hint style="info" %}
<mark style="color:blue;">**Note:**</mark>

* <mark style="color:blue;">The S model does not support RAID.</mark>
* <mark style="color:blue;">Instances with OS of ESXi or Windows can not communicate with others in a VPC.</mark>
{% endhint %}

1. Select the region, city and zone. \
   If you haven't found the location you need, click **Restock Inventory** on the right.
2. Select your preferred specification.\
   If you haven't found the specification you need, click **Restock Inventory** on the right.
3. Choose your desired operating system.
4.  Choose RAID level

    RAID (Redundant Array of Independent Disks) creates a single usable data disk, where several physical disks are combined into an array for better speed and fault tolerance. Zenlayer supports the most common RAID types: 0, 1, 5, and 10.

    Choose RAID 0 for a single hard drive, RAID 1 for two hard drives, and RAID 5 for three or more hard drives. You can also go to customized RAID settings for advanced configurations.
5. Create partitions if needed.\
   Default partitioning style depends on your selected operating system. Please refer to the official documentation of your selected OS for more details.
6. Select the login method for your instance.\
   You can use system-generated root password, SSH keys, or your customized password to log in to your instance.
7. Label your instance and select your desired quantity.\
   You can create instances in batches and give each of your instances an identified name that you can remember.&#x20;

## **Step 3 - Configure the network information for your instance**

1. Set up public network\
   Each instance includes a default amount of bandwidth (for example, 10M, 30M, 50M, or 100M, depending on your selected location and size). If extra bandwidth is needed, please select a pricing model. See [**Bare Metal Cloud Pricing**](../../pricing/bare-metal-cloud-pricing/) for more details.&#x20;
2.  Set up public network\
    Each instance includes a default amount of bandwidth (for example, 10M, 30M, 50M, or 100M, depending on your selected location and size). If extra bandwidth is needed, please select a pricing model. See [**Bare Metal Cloud Pricing**](../../pricing/bare-metal-cloud-pricing/) for more details.&#x20;

    * Flat Rate

    Drag to select your desired bandwidth cap for your stable business with little bursty traffic, and use unlimited data transfer.

    * Data Transfer

    You are billed according to your selected data transfer package, and data consumed beyond your selected package will be charged by the hour. We highly recommend that you select a package that meets the actual needs of your business.\
    You can also set the upper limit of public network bandwidth to control traffic usage in case of extra high charge. If you don’t set the bandwidth cap, it will be the default value.
3. Set up private network\
   If you need your instance to run in a VPC, create or select a VPC and a subnet. See [**Create a VPC**](create-a-virtual-private-cloud.md) for more details.

## **Step 4 - Select your add-ons**

* If your selected zone supports a DDoS protected EIP to be assigned to your instance, you can add this service here.
* Select a resource group for your instance.

## **Step 5 - Check and pay your order**

1. Review your order summary. If there are no problems, please read through the policy documents and check the agreement.
2. Click **Confirm Order** and pay the order. Installation typically takes a few minutes. Once installation is complete, your instance is ready for use.

{% hint style="info" %}
<mark style="color:blue;">**Note:**</mark>\ <mark style="color:blue;">Please pay close attention to your email as zenConsole will send you the IPMI password.</mark>&#x20;
{% endhint %}

## **What to do next**

You can check and manage your BMC instances in **Bare Metal** > **Bare Metal Instance**.&#x20;

1. In **Actions**, you can log in to IPMI, power on/off instances, reboot instances, change OS, view order and unsubscribe/resubscribe instances.
2. Click the name of instance, and you can perform the following operations:
   * View bandwidth usage and other basic information in **Overview**.
   * View bandwidth usage and other basic information in **Overview**.
   * View public and private networking settings, and change bandwidth under Flat Rate pricing model, attach a VPC, or create an elastic IP, and so on in **Networking**.&#x20;
   * Reinstall operating system and change basic configurations of your instance in **OS**.
   * Log in to IPMI or change IPMI password in [**IPMI**](../overview/ipmi.md)**.**
   * Power on, power off or reboot your instance in **State.**
   * Unsubscribe/resubscribe your instance in **Unsubscribe**.&#x20;

