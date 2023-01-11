---
description: >-
  The following steps are applicable to Cloud-to-IDC connections based on our
  Layer 3 SDN backbone network.
---

# Create a Layer 3 Connection

After creating a cloud router, you can contact Zenlayer support or your data center operator to establish a cross connect.



## Procedures

### **Step 1 - Sign in to zenConsole**

1. Use your email address and password to sign in to **** [**zenConsole**](https://console.zenlayer.com/).
2. On the left navigation panel, go to **Cloud Networking** > **Cloud Router** > **Create Cloud Router**.



### **Step 2 - Label Your Cloud Router**

Label your cloud router and add a description for identification.



### **Step 3 - Add Access Points**

Add at least 2 access points. You will need to select **Public Cloud** as the **Access Point Type** for one of your access points.

<figure><img src="../../../.gitbook/assets/Article_1 (6).jpg" alt=""><figcaption><p>Add Access Point</p></figcaption></figure>

1. Select **Public Cloud** as the Access Point Type.\

2. Select your cloud provider. \
   zenConsole supports AWS and Tencent Cloud connection.\
   After creating the connection, see [**Validate Connection in Public Cloud**](validate-connection-in-public-cloud.md) for more details.\

3. Select the cloud connect closest to your infrastructure on the public cloud to guarantee high network performance.\
   \
   <img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>
   * <mark style="color:blue;">If your cloud provider is not AWS or Tencent Cloud, please contact Zenlayer support to create your cloud router.</mark>
   * <mark style="color:blue;">If all locations are too far away, please contact Zenlayer support to create your new cloud connect.</mark>\ <mark style="color:blue;"></mark>
4. Label your cloud connect for identification.\

5. Enter your AWS account ID – a 12-digit number like 123456789012.\

6. Select or enter the VLAN ID of your cloud. Data will be transmitted in the corresponding VLAN.\

7. Select the bandwidth cap of your cloud router from 1 Mbps to 500 Mbps.\

8.  Configure the routing information.



    <figure><img src="../../../.gitbook/assets/Article_2 (2).jpg" alt=""><figcaption><p>Configure Routing Information</p></figcaption></figure>

    * **BGP Routing**\
      ****BGP (border gateway protocol) is usually used to maintain complex networks that contain many routers. BGP divides an intranet into groups of routers, or AS (automated systems), which have trusted routes between them. You must define the AS number on the routers in your network and configure at least one group that includes at least one peer. BGP supports MD5 (message-digest algorithm 5) to secure messages.
    * **Static Routing**\
      ****Static routing is generally used in smaller networks that contain only a couple of routers, or when security is an issue. Each static router must be configured and maintained separately.


9. Select **Data Center** as the Access Point Type.\
   Please see [#step-3-add-access-points](../data-center-connection/create-a-layer-3-connection.md#step-3-add-access-points "mention") in [**Layer 3 IDC-to-IDC connections**](../data-center-connection/create-a-layer-3-connection.md) for specific detailed steps.



### **Step 4 - Confirm Your Configuration**

1. Confirm the billing details and read through the policy.
2. Click **Create** to deploy your cloud router.



## **Result**

After your cross connect is established, the corresponding port state will change to **Active** and you will receive a notification email. Once all ports are active and you have accepted the connection on AWS Console, your cloud router state will become **Active**.\


<mark style="color:blue;">****</mark><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

1. <mark style="color:blue;">Billing for cloud router will not start until cloud connect and all ports are active, and your connection is active.</mark>
2. <mark style="color:blue;">Billing for your port will start:</mark>
   * <mark style="color:blue;">when the port is active.</mark>
   * <mark style="color:blue;">15 days after you submit the order – whether or not your cross connect has been established.</mark>

<mark style="color:blue;"></mark>
