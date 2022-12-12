# Cloud Router Pricing

Cloud router may involve the following pricing items (depends on the types of access point you will add to the cloud router):

* [**Port**](port-pricing.md)****
* ****[**AWS hosted connection**](aws-hosted-connection-pricing.md)****
* Cloud backbone

This chapter only focuses on the pricing rules of cloud backbone.

## **Billing Method**

Pay-as-you-go: The cost of the previous day is deducted at 1 a.m. (UTC+0). You are responsible for the cost of the entire day as long as service is active at any point during the day.&#x20;

### **Billing Start Time**

Billing on cloud backbone starts as soon as the cloud router is created successfully.

### **Price**

Depends on how many points you will add and the access bandwidth that you select. \
You will be able to see specific price when placing the order on zenConsole.



## **Service Upgrade & Downgrade**

### Increase access bandwidth of existing points or add new points

The new price will take into effect immediately and applied on the day of your confirmed change.

### Decrease access bandwidth of existing points or delete points

The new price will take into effect the day after you confirmed change. You are permitted to downgrade your services up to 3 times per month.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">AWS hosted connection provisions connectivity on demand (50M, 100M, 200M, 300M, 400M, 500M, 1G, 2G, 5G, or 10G) over pre-provisioned network circuits. Your hosted connection is determined automatically (and cannot be changed) according to the access bandwidth you select.</mark>&#x20;

<mark style="color:blue;">For example, if the access bandwidth is 80M, then your hosted connection will be 100M. Therefore you will only be able to change the access bandwidth under the hosted connection.</mark>
{% endhint %}



## **Deletion**

* You can cancel your cloud router at any point instantly.&#x20;
* You will be responsible for accrued costs up to and through the day of the service deletion request.&#x20;
* Your cloud router will be retained for 2 days, during which you can recover it manually.

You can go to **Billing** > **Invoices** to view real-time and historic billing.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">The associated ports of your cloud router's points will not be deleted synchronously and billing for ports will continue until you delete them also.</mark>
* <mark style="color:blue;">Billing for AWS hosted connection by Zenlayer will stop synchronously once you delete the cloud router. But the billing by AWS will continue until you delete the hosted connection also on your AWS Console.</mark>
{% endhint %}



## **FAQ**

### **What happens when you no longer have sufficient balance to continue a** cloud router**?**

<figure><img src="../../.gitbook/assets/Article_1 (20).jpg" alt=""><figcaption><p>A Cloud Router Lifecycle</p></figcaption></figure>

#### 1. Protection Stage (2 days since you run out of account balance)

* Your ports, AWS hosted connections and cloud backbone will continue to be active during the protection stage.
* A reminder email will be sent to users with AdministratorAccess and finance roles to refill account balance in order to continue use.

#### 2. Suspension Stage (2 days after the protection stage)

* Your ports, AWS hosted connections and cloud backbone will be suspended, and a suspension notice email will be sent to users with AdministratorAccess and finance roles.
* During this grace period, we will still retain your resources. After your account balance is refilled, you may continue to use them. &#x20;

#### 3. Recycle Stage (After the suspension stage)

* All your ports, AWS hosted connections and cloud backbones will be destroyed, and you will not be able to recover them.
* A final notice email will be sent to users with AdministratorAccess and finance roles.

