---
description: >-
  After both source and destination point configurations, you need to configure
  the network information of your access points, and the name of your private
  connect.
---

# Configure Network Information

<figure><img src="../../../.gitbook/assets/image (16) (1).png" alt=""><figcaption><p>Network Configuration</p></figcaption></figure>

1. Select or enter the VLAN ID of your source and destination ports. Data will be transmitted in the corresponding VLAN.\
   The system will assign a VLAN ID by default, but you can also choose your own between 2-4000.
2. Select the bandwidth cap of your private connect.
3. Label your private connect for identification.
4. Confirm the billing details and read through the policy.
5. Click **Create** to deploy your private connect.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">If you connect to a public cloud, the public cloud usually provides different access bandwidth specifications as follows. You will be charged for the nearest cap higher than your configuration as the cloud connect bandwidth. Your actual access bandwidth of the private connect is still what you have configured.</mark>
  * <mark style="color:blue;">AWS: 50 Mbps, 100 Mbps, 200 Mbps, 300 Mbps, 400 Mbps, 500 Mbps, 1 Gbps, 2 Gbps, 5 Gbps, and 10 Gbps.</mark>
  * <mark style="color:blue;">Tencent Cloud: 50 Mbps, 100 Mbps, 200 Mbps, 300 Mbps, 400 Mbps, 500 Mbps, 1 Gbps, 2 Gbps, 5 Gbps, 8 Gbps, 10 Gbps, 40 Gbps, and 100 Gbps.</mark>&#x20;
  * <mark style="color:blue;">Google Cloud: 50 Mbps, 100 Mbps, 200 Mbps, 300 Mbps, 400 Mbps, 500 Mbps, 1 Gbps, 2 Gbps, 5 Gbps, 10 Gbps, 20 Gbps and 50 Gbps.</mark>&#x20;
* <mark style="color:blue;">After creating your private connect, see</mark> [<mark style="color:purple;">What to Do Next</mark>](./#what-to-do-next) <mark style="color:blue;">to active your points.</mark>
* <mark style="color:blue;">Check the</mark> [<mark style="color:purple;">states</mark>](./#result) <mark style="color:blue;">of your private connect to see whether it is active.</mark>
{% endhint %}

