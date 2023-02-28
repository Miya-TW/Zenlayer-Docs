---
description: >-
  The following configurations are applicable to VPC connection. You can connect
  to an existing VPC created before, or create a new one.
---

# Select a VPC as Access Point

<figure><img src="../../../.gitbook/assets/image (7) (1).png" alt=""><figcaption><p>VPC Connection</p></figcaption></figure>

If you have created a [VPC](../../../bare-metal-cloud/overview/virtual-private-cloud.md), and you want resources in this VPC can communicate with other resources in your data center or infrastructures in your public cloud, add this VPC as an access point into a cloud router.

If you haven't got your desired VPC, you can create a new one. See [VPC creation](../../../bare-metal-cloud/get-started/create-a-virtual-private-cloud.md) for more details.

{% hint style="info" %}
**Note**

There are subnets in a VPC and instances in subnets with the same IP range can not communicate with each other. Please plan the IP ranges of your subnets reasonably in advance in case of abnormal connection.
{% endhint %}

