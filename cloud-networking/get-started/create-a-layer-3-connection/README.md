---
description: >-
  The following steps are applicable to connections with several access points
  of IDCs, public clouds or VPCs based on Layer 3 SDN backbone network.
---

# Create a Layer 3 Connection

If you need a Layer 3 network connection - the [cloud router](../../overview/concepts.md#cloud-router), you can follow the steps as shown below.



## Prerequisites

* You have [signed up an account](../../../platform/account-management/create-an-account.md) with your email and sign in to **** [**zenConsole**](https://console.zenlayer.com/).
* If you need to connect to your cloud services, your public cloud provider should be one of the following: AWS and Tencent Cloud.\
  More public cloud providers will be supported soon.
* For VPC connection, instances in subnets with the same IP range can not communicate with each other. Please plan the IP ranges of your subnets reasonably in advance in case of abnormal connection.



## Procedures

On the upper left corner of zenConsole, go to **Products** > **Cloud Networking** > **Cloud Router** > [**Create Cloud Router**](https://console.zenlayer.com/sdn/router/create). \
The overall steps of creating a cloud router is shown below. For detailed operations, please refer to the links of specific chapters.

<figure><img src="../../../.gitbook/assets/image (14).png" alt=""><figcaption><p>Create a Cloud Router</p></figcaption></figure>

### 1. Label Your Cloud Router&#x20;

<figure><img src="../../../.gitbook/assets/image (9) (1).png" alt=""><figcaption></figcaption></figure>

Label your cloud router for identification. Click **Continue** to add access points.&#x20;



### 2. Add Access Points

You need to add at least 2 access points and configure routing and network information to get started. You will be able to make updates in the future.\
You may have the following options to add:

* [Data center](select-a-data-center-as-access-point.md)
* [Public cloud](select-a-public-cloud-as-access-point.md)
* [VPC](select-a-vpc-as-access-point.md)



### 3. Configure Routing

If you add access points like data centers or public clouds, you need to configure routing protocols to achieve network communication. If you add a VPC, go to configure network directly.

You may have the following options, and if your device supports Border Gateway Protocol (BGP), we recommend using BGP to take care of network segment changes.

* [BGP routing](configure-routing-information.md#bgp-routing)
* [Static routing](configure-routing-information.md#static-routing)



### 4. Configure Network

[Configure the network information](configure-network-information.md) of your cloud router.\
You need to configure the access bandwidth of your access point. &#x20;



### What to Do Next

More operations offline or on the public cloud console.

#### For the Public Cloud Point

[Validate your cloud connect](../validate-connection-in-public-cloud.md) on the corresponding console of your public cloud provider.

#### For the Data Center Point

Contact Zenlayer Support or your data center operator to establish a cross connect offline.



### Result

After your cross connect is established offline and your cloud connect is validated on the public cloud console, the states of corresponding points will change into **Active** and you will receive a notification email.

Once the states of all access points are **Active**, your cloud router state will become **Active**.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">Billing for cloud router will not start until all access points are active, and your connection is active.</mark>
* <mark style="color:blue;">Billing for your port will start:</mark>
  * <mark style="color:blue;">when the port is active.</mark>
  * <mark style="color:blue;">15 days after you submit the order – whether or not your cloud router has been established.</mark>
* <mark style="color:blue;">Billing for your cloud connect will start:</mark>\ <mark style="color:blue;">once you have validated your cloud connect on the public cloud console.</mark>
{% endhint %}

<mark style="color:blue;">****</mark>
