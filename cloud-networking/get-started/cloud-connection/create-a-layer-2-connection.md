---
description: >-
  The following steps are applicable to Cloud-to-IDC connections based on our
  Layer 2 SDN backbone network.
---

# Create a Layer 2 Connection

After creating a private connect, you can contact Zenlayer support or your data center operator to establish a cross connect.



## Procedures

### **Step 1 - Sign in and go to create**

1. Use your email address and password to sign in to **** [**zenConsole**](https://console.zenlayer.com/).
2. On the left navigation panel, go to **Cloud Networking** > **Private Connect** > **Create Cloud Connect**.



### **Step 2  Configure cloud connect**

<figure><img src="../../../.gitbook/assets/Article_1 (19).jpg" alt=""><figcaption><p><strong>Layer-2 Cloud Connect</strong> </p></figcaption></figure>

1. Select your cloud provider. \
   zenConsole supports AWS and Tencent Cloud connection.\
   After creating the connection, see [**Validate Connection in Public Cloud**](validate-connection-in-public-cloud.md) for more details.
2.  Select the cloud connect closest to your infrastructure on the public cloud to guarantee high network performance.\
    \
    <img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

    * <mark style="color:blue;">If your public cloud provider is not AWS or Tencent Cloud, please contact Zenlayer support to create your cloud router.</mark>
    * <mark style="color:blue;">If all locations are too far away, please contact Zenlayer support to create your new cloud connect.</mark>


3. Label your cloud connect for identification.
4. Enter your cloud account ID – a 12-digit number like 123456789012.



### **Step 3 - Configure the Destination Port**

<figure><img src="../../../.gitbook/assets/Article_2 (5).jpg" alt=""><figcaption><p>Configure Destination Port</p></figcaption></figure>

Select a port closest to your data center.

#### **Existing Port**

If you have an established cross connect to Zenlayer Cloud Networking, you can select your existing port.

#### **New Port**

If this is your first time creating a cloud connect, you will need to select a new port.

1. Select the port location closest to one of your data centers.
2. Select the port rate. 1 Gbps and 10 Gbps are supported.\
   \
   <img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>\ <mark style="color:blue;">To future-proof your business, a 10 Gbps port rate is recommended.</mark>\
   __
3. Label your port for identification.
4.  Enter the legal business name of the authorized party. You will receive an LOA (letter of authorization) that is used to establish your cross connect.\


    <figure><img src="../../../.gitbook/assets/Article_2 (3) (1).jpg" alt=""><figcaption><p>Download LOA File</p></figcaption></figure>

    <mark style="color:blue;">****</mark><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

    * <mark style="color:blue;">The LOA will be emailed to you as an attachment 2 to 3 days after you submit your new port order. You can also download your LOA in the</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Port View**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">on zenConsole.</mark>
    * <mark style="color:blue;">The LOA will expire in 30 days. Please establish your cross connect as soon as possible.</mark>



### **Step 4 - Configure the Connection**

<figure><img src="../../../.gitbook/assets/Article_4 (1).jpg" alt=""><figcaption><p>Configure Connection</p></figcaption></figure>

Configure the connection between the cloud and the destination port.

1. Select or enter the VLAN ID of your cloud and destination port. Data will be transmitted in the corresponding VLAN.
2. Select the bandwidth cap of your private connect from 1 Mbps to 500 Mbps.
3. Label your private connect for identification.



### **Step 5 - Confirm Your Configuration**

1. Confirm the billing details and read through the policy.
2. Click **Create** to deploy your private connect.

****

## **Result**

After your cross connect is established, the corresponding port state will change to **Active** and you will receive a notification email. Once the destination port is active and you have validated the connection on public cloud Console, your private connect state will become **Active**.\ <mark style="color:blue;">****</mark>

<mark style="color:blue;">****</mark><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

1. <mark style="color:blue;">Billing for private connect will not start until both the cloud connect and destination port are active, and your connection is active.</mark>
2. <mark style="color:blue;">Billing for your port will start:</mark>
   * <mark style="color:blue;">when the port is active.</mark>
   * <mark style="color:blue;">15 days after you submit the order – whether or not your cross connect has been established.</mark>

