# Private Connect Pricing

Private Connect may involve the following pricing items (depends on the source and destination port you will add):

* [**Port**](port-pricing.md)****
* ****[**AWS hosted connection**](aws-hosted-connection-pricing.md)****
* Connection bandwidth

This chapter only focuses on the pricing rules of connection bandwidth.

<figure><img src="../../.gitbook/assets/Article_1 (1).jpg" alt=""><figcaption><p>A Private Connect</p></figcaption></figure>

## **Billing Method**

Pay-as-you-go: The cost of the previous day will be deducted at 1 a.m. (UTC+0), and less than one day will be calculated as one day.

### **Billing Start Time**

Billing starts only when the private connect’s two ends are active and the entire network is activated.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">Port connecting to your on-premises data center: The port will be active when the cross connect is completed.</mark>
* <mark style="color:blue;">AWS hosted connection: The hosted connection is active when you accept it on AWS Console.</mark>
{% endhint %}

### **Price**

Depends on your selected bandwidth cap and the sites of the two ends. \
You will be able to see specific price when placing the order on zenConsole.



## **Service Upgrade & Downgrade**

### Increase Bandwidth Cap

The new price will take into effect immediately and applied on the day of your confirmed change.

### Decrease Bandwidth Cap

The new price will take into effect the day after you confirmed change. You are permitted to decrease your bandwidth cap up to 3 times per month.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">AWS hosted connection provisions connectivity on demand (50M, 100M, 200M, 300M, 400M, 500M, 1G, 2G, 5G, or 10G) over pre-provisioned network circuits. Your hosted connection is determined automatically (and cannot be changed) according to the connection bandwidth you select.</mark>&#x20;

<mark style="color:blue;">For example, if the connection bandwidth is 80M, then your hosted connection will be 100M. Therefore you will only be able to change the access bandwidth under the hosted connection.</mark>
{% endhint %}



## Deletion

* You can cancel your private connect at any point instantly.&#x20;
* You will be responsible for accrued costs up to and through the day of the service deletion request.&#x20;
* Your private connect will be retained for 2 days, during which you can recover it manually.

You can go to **Billing** > **Invoices** to view real-time and historic billing.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">The associated ports of your private connect will not be deleted synchronously and billing for ports will continue until you delete them also.</mark>
* <mark style="color:blue;">Billing for AWS hosted connection by Zenlayer will stop synchronously once you delete the private connect. But the billing by AWS will continue until you delete the hosted connection also on your AWS Console.</mark>
{% endhint %}



## **FAQ**

### **What happens when you no longer have sufficient balance to continue a** private connect**?**

Once you no longer have remaining account balance (<0), the following process will ensue:

<figure><img src="../../.gitbook/assets/Article_2 (9).jpg" alt=""><figcaption><p>A Private Connect Lifecycle</p></figcaption></figure>

#### 1. Protection Stage (2 days since you run out of account balance)

* Your ports, AWS hosted connections and private connects will continue to be active during the protection stage.
* A reminder email will be sent to users with _AdministratorAccess_ and _Finance_ roles to refill account balance in order to continue use.

#### 2. Suspension Stage (2 days after the protection stage)

* Your ports, AWS hosted connections and private connects will be suspended, and a suspension notice email will be sent to users with _AdministratorAccess_ and _Finance_ roles.
* During this grace period, we will still retain your connects. After your account balance is refilled, you may continue to use your ports.&#x20;

#### 3. Recycle Stage (After the suspension stage)

* All your ports, AWS hosted connections and private connects will be destroyed, and you will not be able to recover them.
* A final notice email will be sent to users with _AdministratorAccess_ and _Finance_ roles.

