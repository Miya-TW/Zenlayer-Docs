# Create a Virtual Private Cloud

## **Step 1 - Sign in to zenConsole**

1. Use your email address and password to sign in to [**zenConsole**](https://console.zenlayer.com/dashboard).
2. On the left navigation panel, go to **Compute** > **Bare Metal** > **Virtual Private Cloud** > **Create Virtual Private Cloud**.

## **Step 2 - Configure basic information of your VPC**

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">VPC label name can only contain alphanumeric characters, dashes, and periods.</mark>
* <mark style="color:blue;">The private IP range cannot be changed once configured. You are highly recommended to plan the network in advance.</mark>
* <mark style="color:blue;">See</mark> [<mark style="color:purple;">**Create a Subnet**</mark>](create-a-subnet.md) <mark style="color:blue;">for more details.</mark>
{% endhint %}

1. Select a location where you need your VPC.\
   You can create a VPC in the availability region. An availability region consists of several bare metal zones, for example, Atl-A and Atl-B.
2. Configure the private IP range.\
   After you configure the private IP range for your VPC, the resources in this VPC will be assigned private IP addresses for secure communication within the specified IP range.
3. Label your VPC.\
   VPC label name can only contain alphanumeric characters, dashes, and periods.
4. Create a subnet.\
   You can specify a subset of your VPC IP range for your subnet.
5. Select a resource group.\
   Resources in the resource group allocated to your VPC can communicate with each other.
6. Click **Create** to confirm the configuration.

## **What to do next**

You can check and manage your VPC in **Bare Metal** > **Virtual Private Cloud**.&#x20;

* Click **Delete** to delete your VPC
* Click **Add Subnet** to add a subnet to the VPC
* Click **Add Instance** to add instances to a subnet

