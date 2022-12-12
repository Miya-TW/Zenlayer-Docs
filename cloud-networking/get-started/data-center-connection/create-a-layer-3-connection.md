---
description: >-
  The following steps are applicable to IDC-to-IDC connections based on our
  Layer 3 SDN backbone network.
---

# Create a Layer 3 Connection

After creating your cloud router, you can contact Zenlayer support or your data center operator to establish a cross connect.



## Procedures

### **Step 1 - Sign in and go to create**

1. Use your email address and password to sign in to **** [**zenConsole**](https://console.zenlayer.com/).
2. On the left navigation panel, go to **Cloud Networking** > **Cloud Router** > **Create Cloud Router**.



### **Step 2  Label Your Cloud Router**

Label your cloud router and add a description for identification.



### **Step 3  Add Access Points**

Add at least 2 access points by selecting **Data Center** as the **Access Point Type**.

<figure><img src="../../../.gitbook/assets/Article_1 (18).jpg" alt=""><figcaption><p>Layer-3 Data Center Connection</p></figcaption></figure>

#### 1. Select **Data Center** as the Access Point Type.

#### 2. Select a port closest to your data center.

* **Existing Port**\
  ****If you have an established cross connect to Zenlayer Cloud Networking, you can select your existing port.
* **New Port**\
  ****If this is your first time creating a private connect, you will need to select a new port.

&#x20;     1\) **** Select the port location closest to one of your data centers.\
\
&#x20;     2\) Select the port rate. 1 Gbps and 10 Gbps are supported.  \
\
&#x20;     <img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>\
&#x20;     <mark style="color:blue;">To future-proof your business, a 10 Gbps port rate is recommended.</mark>

&#x20;     3\) Label your port for identification.\
\
&#x20;     4\) Enter the legal business name of the authorized party. \
&#x20;          You will receive an LOA (letter of authorization) that is used to establish your cross connect.

<figure><img src="../../../.gitbook/assets/Article_2 (8).jpg" alt=""><figcaption><p>Download LOA File</p></figcaption></figure>

&#x20;      <mark style="color:blue;">****</mark>       <img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">The LOA will be emailed to you as an attachment 2 to 3 days after you submit your new port order. You can also download your LOA in the</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Port View**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">on zenConsole.</mark>
* <mark style="color:blue;">The LOA will expire in 30 days. Please establish your cross connect as soon as possible.</mark>

#### 3. Select or enter the VLAN ID of your port. Data will be transmitted in the corresponding VLAN.

#### 4. Select the bandwidth cap of your cloud router from 1 Mbps to 500 Mbps.

#### 5. Configure the routing information.

<figure><img src="../../../.gitbook/assets/Article_3 (1).jpg" alt=""><figcaption><p>Configure Routing Information</p></figcaption></figure>

* **BGP Routing**\
  ****BGP (border gateway protocol) is usually used to maintain complex networks that contain many routers. BGP divides an intranet into groups of routers, or AS (automated systems), which have trusted routes between them. You must define the AS number on the routers in your network and configure at least one group that includes at least one peer. BGP supports MD5 (message-digest algorithm 5) to secure messages.
* **Static Routing**\
  ****Static routing is generally used in smaller networks that contain only a couple of routers, or when security is an issue. Each static router must be configured and maintained separately.

#### 6. Add other access points following the steps above.



### **Step 4 - Confirm Your Configuration**

1. Confirm the billing details and read through the policy.
2. Click **Create** to deploy your cloud router.



## **Result**

After your cross connect is established, the corresponding port state will change to **Active** and you will receive a notification email. Once all ports are active, your cloud router state will become **Active**.\


<mark style="color:blue;">****</mark><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>

1. <mark style="color:blue;">Billing for cloud router will not start until all ports are active, and your connection is active.</mark>
2. <mark style="color:blue;">Billing for your port will start:</mark>
   * <mark style="color:blue;">when the port is active.</mark>
   * <mark style="color:blue;">15 days after you submit the order – whether or not your cross connect has been established.</mark>

