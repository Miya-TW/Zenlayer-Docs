# AWS Hosted Connection Pricing

## **Billing Method**

Pay-as-you-go: The cost of the previous day will be deducted at 1 a.m. (UTC+0), and less than one day will be calculated as one day.

### **Billing Start Time**

Billing on AWS hosted connection starts as soon as you accept the request on AWS Console initiated by Zenlayer.

### **Price**

Depends on the bandwidth size of the hosted connection, which is determined automatically according to the connection bandwidth of Point to Point network or the access bandwidth of Cloud Router's point.&#x20;

For example, if your connection bandwidth is 80M, then your hosted connection will be 100M.\
You will be able to see price details when placing the order on zenConsole.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>\ <mark style="color:blue;">AWS hosted connection provisions connectivity on demand (50M, 100M, 200M, 300M, 400M, 500M, 1G, 2G, 5G, or 10G) over pre-provisioned network circuits.</mark>
{% endhint %}



## **Deletion**

* Before you accept the hosted connection request on AWS Console, you can delete it directly on zenConsole and the associated private connect will be deleted synchronously.
* If you have accepted the hosted connection request on AWS Console, after you delete it and the associated private connect on zenConsole, you also need to delete the same on AWS Console by yourself, in order to stop the billing by AWS.

You can go to **Billing** > **Invoices** to view real-time and historic billing.



## **FAQ**

### **What happens when you no longer have sufficient balance to continue an** AWS hosted connection**?**

Once you no longer have remaining account balance (<0), the following process will ensue:

<figure><img src="../../.gitbook/assets/Article_1 (20) (1).jpg" alt=""><figcaption><p>An AWS Hosted Connection Lifecycle</p></figcaption></figure>

#### 1. Protection Stage (2 days since you run out of account balance)

* Your hosted connection will continue to be active during the protection stage.
* A reminder email will be sent to users with _AdministratorAccess_ and _Finance_ roles to refill account balance in order to continue use.

#### 2. Suspension Stage (2 days after the protection stage)

* Your hosted connection will be suspended, and a suspension notice email will be sent to users with _AdministratorAccess_ and _Finance_ roles.
* During this grace period, we will still retain your hosted connection. After your account balance is refilled, you may continue to use your hosted connection.&#x20;

#### 3. Recycle Stage (After the suspension stage)

* Your hosted connection will be destroyed, and you will not be able to recover it.
* A final notice email will be sent to users with _AdministratorAccess_ and _Finance_ roles.

