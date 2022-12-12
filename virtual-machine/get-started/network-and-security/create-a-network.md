---
description: >-
  You can configure virtual private networks for your virtual machine instances
  on zenConsole to realize the instance isolation.
---

# Create a Network

## Prerequisites

You can create 2 networks in one location at most. After creating a network, you can create an instance and attach it to the network.



## Procedures

1. Log in to [**zenConsole**](https://console.zenlayer.com/).
2. Go to **Compute** > **Virtual Machine** > **Network** and click **Create Network**.
3. Identify your network.\
   \
   <img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>\ <mark style="color:blue;">The name must be 2 to 128 characters in length, containing only letters, numbers, hyphens (-) and periods (.). It must start with a letter, but not http:// or https://.</mark>\ <mark style="color:blue;"></mark>
4. Select the location you need your network.
5. Configure the IP address of your network. 10.0.0.0/8, 172.16.0.0/12 and 192.168.0.0/16 are supported.
6. Add a subnet in your network. See **** [**Create a Subnet**](create-a-subnet.md) for more details.\
   \
   <img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>\ <mark style="color:blue;">You can refer to</mark> <mark style="color:blue;"></mark>_<mark style="color:blue;"></mark>_ [<mark style="color:blue;"><mark style="color:purple;">**Network Planning**<mark style="color:purple;"></mark>](../../overview/vpc-and-subnet-planning.md) <mark style="color:blue;">to reasonably configure your network and subnet.</mark>\ <mark style="color:blue;"></mark>
7. Click **Create** to create a network.
8. _<mark style="color:green;">(Optional)</mark>_ <mark style="color:green;"></mark><mark style="color:green;"></mark> Go to **Action** > **Delete** to delete the network if no subnets or instances added to it.

