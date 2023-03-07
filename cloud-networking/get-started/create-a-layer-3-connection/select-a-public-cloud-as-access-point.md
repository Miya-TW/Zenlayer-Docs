---
description: >-
  The following configurations are applicable to public cloud connection. You
  can connect to AWS, Tencent Cloud or Google Cloud. More public cloud providers
  will be supported soon.
---

# Select a Public Cloud as Access Point

<figure><img src="../../../.gitbook/assets/image (7).png" alt=""><figcaption><p>Public Cloud Connection</p></figcaption></figure>

1. Select your cloud provider. \
   zenConsole supports AWS, Tencent Cloud and Google Cloud connection for now.
2. _<mark style="color:green;">(Only for Google Cloud)</mark>_ For Google Cloud connection, you need to provide your [**pairing key**](https://cloud.google.com/network-connectivity/docs/interconnect/concepts/terminology#pairingkey) obtained from Google Cloud first. Zenlayer will find a closest location to match according to your pairing key. Please ensure the format is correct. \
   See [<mark style="color:blue;">**Validate Cloud Connection**</mark>](../validate-connection-in-public-cloud.md) to know how to obtain a pairing key.
3.  Select the cloud connect closest to your infrastructures on the public cloud to guarantee high network performance.

    <img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

    * <mark style="color:blue;">If all locations are too far away, please contact Zenlayer support to create your new cloud connect.</mark>
    * <mark style="color:blue;">If your public cloud provider is not AWS, Tencent Cloud or Google Cloud, please contact Zenlayer support to create your cloud router.</mark>
4. Label your cloud connect for identification.
5. Enter your cloud account ID – a 12-digit number like 123456789012.
6. Configure a VLAN ID, and data will be transmitted in the corresponding VLAN.\
   The system will assign a VLAN ID by default. If you want to customize it, choose a VLAN ID within 2 to 4000.



## What to Do Next

[Validate your cloud connect](../validate-connection-in-public-cloud.md) on the corresponding console of your public cloud provider.

