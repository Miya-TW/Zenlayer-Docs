---
description: >-
  The following steps are applicable to IDC-to-IDC connections based on our
  Layer 2 SDN backbone network.
---

# Create a Layer 2 Connection

After creating a private connect, you can contact Zenlayer support or your data center operator to establish a cross connect.



## Procedures

### **Step 1 - Sign in and go to create**

1. Use your email address and password to sign in to [**zenConsole**](https://console.zenlayer.com/).
2. On the left navigation panel, go to **Cloud Networking** > **Private Connect** > **Create Data Center Interconnect**.



### **Step 2 - Configure the Source and Destination Ports**

#### 1. Select a source port closest to your one of your data centers.

<figure><img src="../../../.gitbook/assets/Article_1 (14).jpg" alt=""><figcaption><p>Layer-2 Data Center Connection</p></figcaption></figure>

**Existing Port**\
****If you have an established cross connect to Zenlayer Cloud Networking, you can select your existing port.&#x20;

**New Port**\
****If this is your first time creating a private connect, you will need to select a new port.

1\) Select the port location closest to one of your data centers.\
\
2\) Select the port rate. 1 Gbps and 10 Gbps are supported.\
\
<img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>\ <mark style="color:blue;">To future-proof your business, a 10 Gbps port rate is recommended.</mark>\
\
3\) Label your port for identification.\
\
4\) Enter the legal business name of the authorized party. You will receive an LOA (letter of authorization) that is used to establish your cross connect.

<figure><img src="../../../.gitbook/assets/Article_2 (3) (1).jpg" alt=""><figcaption><p>Download LOA File</p></figcaption></figure>

<img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">The LOA will be emailed to you as an attachment 2 to 3 days after you submit your new port order. You can also download your LOA in the</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Port View**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">on zenConsole.</mark>
* <mark style="color:blue;">The LOA will expire in 30 days. Please establish your cross connect as soon as possible.</mark>



#### 2. Select a destination port closest to the other data center.

The steps are the same as selecting a source port above.\


<mark style="color:blue;">****</mark><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>\ <mark style="color:blue;">The lowest port rate of your source port and destination port determines the transmission rate of your private connection.</mark>



### **Step 3 - Configure the Connection**

Configure the connection between the source port and the destination port.

<figure><img src="../../../.gitbook/assets/Article_3 (3).jpg" alt=""><figcaption><p>Configure Connection</p></figcaption></figure>

1. Select or enter the VLAN ID of your source and destination ports. Data will be transmitted in the corresponding VLAN.
2. Select the bandwidth cap of your private connect from 1 Mbps to 500 Mbps.
3. Label your private connect for identification.



### **Step 4 - Confirm Your Configuration**

1. Confirm the billing details and read through the policy.
2. Click **Create** to deploy your private connect.



## **Result**

After your cross connect is established, the corresponding port state will change to **Active** and you will receive a notification email. Once both source and destination ports are active, your private connect state will become **Active**.\


<mark style="color:blue;">****</mark><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

1. <mark style="color:blue;">Billing for private connect will not start until both source and destination ports are active, and your connection is active.</mark>
2. <mark style="color:blue;">Billing for your port will start:</mark>
   * <mark style="color:blue;">when the port is active.</mark>
   * <mark style="color:blue;">15 days after you submit the order – whether or not your cross connect has been established.</mark>

