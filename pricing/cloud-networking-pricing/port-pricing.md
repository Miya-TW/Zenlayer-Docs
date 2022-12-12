# Port Pricing

## **Billing Method**

Pay-as-you-go: The cost of the previous day will be deducted at 1 a.m. (UTC+0), and less than one day will be calculated as one day.

Your port's daily cost depends on the port optics (1Gbps or 10Gbps) and site. You will be able to see price details when placing the order on zenConsole.

Billing starts when one of the following conditions is met:

* The port is active.\
  Once you ordered the port, the LOA (Letter of Authorization) will be sent to you within 2-3 days. With the LOA, you can establish the cross connect to your port. Once the cross connect is completed, the port's status will become active.
* 15 days after the order is placed, regardless of whether the port is active or not.



## **Deletion**

* If billing has yet to begin, you can delete the port directly.
* If billing has begun, you will be responsible for accrued costs up to and through the day of the service deletion request.
* If your port is one end of a private connect or a point of a cloud router, you must delete the private connect or the point of the cloud router before deleting the port.
* Your port will be retained for 2 days, during which you can recover the port manually by clicking **Redeploy** under **Actions** in **Port View**.

You can go to **Billing** > **Invoices** to view real-time and historic billing.



## **FAQ**

### **What happens when you no longer have sufficient balance to continue a port?**

Once you no longer have remaining account balance (<0), the following process will ensue:

<figure><img src="../../.gitbook/assets/Article_1 (14).jpg" alt=""><figcaption><p>A Port Lifecycle</p></figcaption></figure>

#### 1. Protection Stage (2 days since you run out of account balance)

* Your ports will continue to be active during the protection stage.
* A reminder email will be sent to users with _AdministratorAccess_ and _Finance_ roles to refill account balance in order to continue use.

#### 2. Suspension Stage (2 days after the protection stage)

* Your ports will be suspended, and a suspension notice email will be sent to users with _AdministratorAccess_ and _Finance_ roles.
* During this grace period, we will still retain your port. After your account balance is refilled, you may continue to use your ports.&#x20;

#### 3. Recycle Stage (After the suspension stage)

* All your ports will be destroyed, and you will not be able to recover them.
* A final notice email will be sent to users with _AdministratorAccess_ and _Finance_ roles.

