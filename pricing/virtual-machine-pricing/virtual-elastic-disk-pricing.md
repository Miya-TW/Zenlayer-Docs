# Virtual Elastic Disk Pricing

## **Pricing Item**

The pricing item of a virtual elastic disk is the storage space (GB) of the disk. The price varies according to the storage volume and the location. You will see the price when placing the order on zenConsole.



## **Billing Method**

Your virtual elastic disk is subscribed on a 30-day basis and renewed automatically.



## **Unsubscription**

If you will no longer use the a virtual elastic disk, you can go to **Billing** > **Subscriptions** > **Auto Renewal**. Find your virtual elastic disk and click **Unsubscribe**.\
Or go to disk list and click **Cancel Subscription** under **Actions**.

Before the subscription cycle expires, you can click **Resubscribe** to recover the subscription.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">Virtual elastic disk doesn’t support refund on the unused part if being unsubscribed before the subscription cycle expires.</mark>
* <mark style="color:blue;">After being unsubscribed, the virtual elastic disk can be still used till the end of the present subscription cycle.</mark>
{% endhint %}



## **FAQ**

### **What happens when you no longer have sufficient balance to continue a** virtual elastic disk**?**

When your virtual elastic disk fails to renew due to insufficient balance, the following process will ensue:

#### **1. Protection Stage** (24 hours after the renewal failed)

* Your virtual elastic disk will continue to run normally, but you may not create any new one.
* A reminder email will be sent to users with AdministratorAccess and finance roles to refill account balance in order to continue use.

#### **2. Suspension Stage** (72 hours after the protection stage)

* The virtual elastic disk in service will be suspended, and a suspension notice email will be sent to users with AdministratorAccess and finance roles.
* During this grace period, we will still retain your virtual elastic disk resources and data. After your account balance is refilled, zenConsole will renew the subscription automatically as soon as the suspension stage expires, and you will need to manually power on the instance.

#### **3. Recycle Stage** (once the suspension stage expires)

* Your instance resources will be destroyed and recycled, and you will not be able to recover your data.
* A final notice email will be sent to users with AdministratorAccess and finance roles.

