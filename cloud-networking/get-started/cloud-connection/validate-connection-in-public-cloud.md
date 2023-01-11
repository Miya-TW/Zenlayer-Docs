---
description: >-
  After creating a Layer 2 or Layer 3 cloud connection, you need to validate the
  connections on public cloud console.
---

# Validate Connection in Public Cloud

## AWS

If your public cloud provider is AWS, a few minutes after your connection is created, your AWS account will receive your connection information in the **Direct Connect** > **Connections** list.

<figure><img src="../../../.gitbook/assets/Article_5.jpg" alt=""><figcaption><p>Validate Connection on AWS Console</p></figcaption></figure>

1. Click **Accept** to validate your connection.
2. Create a virtual interface and add a BGP peer.\
   Please see [**AWS Documentation**](https://docs.aws.amazon.com/directconnect/latest/UserGuide/create-vif.html) for more details.



## Tencent Cloud

If your public cloud provider is Tencent Cloud, go to Tencent Cloud console.

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Two Kinds of BGP Peering</p></figcaption></figure>

1. [Create a VPC](https://www.tencentcloud.com/document/product/215/31891)
2. [Create a direct connect gateway](https://www.tencentcloud.com/document/product/216/19256) and associate the VPC created in previous step
3.  [Apply for a shared tunnel](https://www.tencentcloud.com/document/product/216/48575)\
    Find the **Connection provider ID** and **Shared tunnel ID** in Tencent Cloud Connection details on zenConsole. \


    <figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Tencent Cloud Connection Details on zenConsole</p></figcaption></figure>

    \
    Fill the **Connection provider ID** and **Shared tunnel ID** into **Basic Configuration** of Shared Dedicated Tunnel creation on Tencent Cloud console, and associate the shared dedicated tunnel to the VPC and gateway created in previous steps.\
    \
    In **Advanced Configuration**, fill the ASN of Tencent Cloud (45090) and ASN of Zenlayer (62610).

