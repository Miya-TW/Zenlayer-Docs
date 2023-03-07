---
description: >-
  The following steps are applicable to connections with two access points of
  IDCs or public clouds based on Layer 2 SDN backbone network.
---

# Create a Layer 2 Connection

If you need a Layer 2 network connection - the [**private connect**](../../overview/concepts.md#private-connect), you can follow the steps as shown below.



## Prerequisites

* You have [**signed up an account**](../../../platform/account-management/create-an-account.md) with your email and sign in to **** [**zenConsole**](https://console.zenlayer.com/).
* If you need to connect to your cloud services, your public cloud provider should be one of the following: AWS, Tencent Cloud and Google Cloud.\
  More public cloud providers will be supported soon.



## Procedures

On the upper left corner of zenConsole, go to **Products** > **Cloud Networking** > **Private Connect** > [**Create Private Connect**](https://console.zenlayer.com/sdn/network/create/ptp). \
The overall steps of creating a private connect is shown below. For detailed operations, please refer to the links of specific chapters.

<figure><img src="../../../.gitbook/assets/image (18).png" alt=""><figcaption><p>Create a Private Connect</p></figcaption></figure>

### 1. Access Point of Source End&#x20;

Select an access point type as the source end of your private connect.\
You may have the following options:

* [Data center](select-a-data-center-as-access-point.md)
* [Public cloud](select-a-public-cloud-as-access-point.md)



### 2. Access Point of Destination End

Select an access point type as the destination end of your private connect.\
You have the same options in the previous step.



### 3. Network Configuration

[Configure the network information](configure-network-information.md) of your private connect.\
You need to configure the VLAN IDs of your access points, bandwidth cap between the points, and the name of your private connect. &#x20;



### What to Do Next

More operations offline or on the public cloud console.

#### For the Public Cloud Point

[Validate your cloud connect](../validate-connection-in-public-cloud.md) on the corresponding console of your public cloud provider.

#### For the Data Center Point

Contact Zenlayer Support or your data center operator to establish a cross connect offline.



### Result

After your cross connect is established offline and your cloud connect is validated on the public cloud console, the states of corresponding points will change into **Active** and you will receive a notification email.

Once the states of both ends are **Active**, your private connect state will become **Active**.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">Billing for private connect will not start until both the source and destination end points are active, and your connection is active.</mark>
* <mark style="color:blue;">Billing for your port will start:</mark>
  * <mark style="color:blue;">when the port is active.</mark>
  * <mark style="color:blue;">15 days after you submit the order – whether or not your cross connect has been established.</mark>
* <mark style="color:blue;">Billing for your cloud connect will start:</mark>\ <mark style="color:blue;">once you have validated your cloud connect on the public cloud console.</mark>
{% endhint %}

