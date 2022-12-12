# Create an Elastic IP

## **Step 1 - Sign in to zenConsole**

1. Use your email address and password to sign in to [**zenConsole**](https://console.zenlayer.com/dashboard).
2. On the left navigation panel, go to **Compute** > **Bare Metal** > **Elastic IP** > **Create Elastic IP**.

## **Step 2 - Configure basic information of your elastic IP**

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">The instance that your elastic IP will be assigned to should be in the same location with the elastic IP.</mark>
{% endhint %}

1. Select a location where you need your elastic IP
2. Choose the IP type
   * Common elastic IP\
     A static IP without DDoS protection.
   * DDoS protected elastic IP\
     A static IP that can scrub malicious traffic so as to prevent network attacks.
3. Assign the elastic IP to an instance\
   You can search the desired instance by label or ID.
4. Select a resource group for the IP\
   You can allocate a resource group to team members. See **** [**Resource Management**](../../platform/team-management/create-a-resource-group.md) for more details.
5. Select your desired quantity

## **Step 3 - Check and pay your order**

Review your order summary and then confirm your order.

See [**Bare Metal Cloud Pricing**](../../pricing/bare-metal-cloud-pricing/) to learn more about elastic IP pricing rules.



## **What to Do Next**

Go to **Bare Metal** > **Elastic IP** > **Actions**, you can reassign, unassign or delete the selected elastic IP.

