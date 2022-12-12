# Create a Subnet

## **Step 1 - Sign in to zenConsole**

1. Use your email address and password to sign in to [**zenConsole**](https://console.zenlayer.com/dashboard).
2. On the left navigation panel, go to **Compute** > **Bare Metal** > **Subnet** > **Create Subnet**.

## **Step 2 - Configure basic information for your subnet**

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">The private IP range cannot be changed once configured. You are highly recommended to plan the network in advance.</mark>
* <mark style="color:blue;">Subnet label name can only contain alphanumeric characters, dashes, and periods.</mark>
{% endhint %}

1. Select a VPC that you want to add your subnet to.\
   If you haven't found the VPC you need, click **Create New** to create a new one.\
   See [**Create a VPC**](create-a-virtual-private-cloud.md) **** for more details.
2. Select a location where you need your subnet.
3. Configure the private IP range.\
   After you configure the private IP range for your subnet, resources in this subnet will be assigned private IP addresses for secure communication within the specified IP range.
4. Label your subnet.
5. Click **Confirm** to create the subnet.

## **What to Do Next**

You can check and manage your subnet in **Bare Metal** > **Subnet**.

* Click VPC name to view details
* Click **Add Instance** to add instances to a subnet

