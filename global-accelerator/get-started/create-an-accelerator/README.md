# Create an Accelerator

If you need to accelerate your services for your end users, you can follow the steps as shown below to create an [accelerator](../../overview.md).



## Prerequisites

You have [signed up an account](../../../platform/account-management/create-an-account.md) with your email and sign in to **** [**zenConsole**](https://console.zenlayer.com/).



## Procedures

On the upper left corner of zenConsole, go to **Products** > **Global Accelerator** > [**Create Accelerator**](https://console.zenlayer.com/gia/project/create).\
The overall steps of creating an accelerator is shown below. For detailed operations, please refer to the links of specific chapters.



### 1. Subscribe a Package

You will first need to select an acceleration package and a billing cycle if it is your time to create an accelerator. You may have the following options: Starter, Plus, Pro and Max, with different specifications. Choose what you need depending on your actual business situation.

<figure><img src="../../../.gitbook/assets/image (8) (1).png" alt=""><figcaption><p>Subscription Package</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">If you are a new user of ZGA, you can try the Starter Package 7 days for free, and you can upgrade to a paid subscription package before your trial expires.</mark>
* <mark style="color:blue;">After clicking</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Choose**</mark><mark style="color:blue;">, you need to select a billing cycle of your package.</mark>
* <mark style="color:blue;">You can upgrade or downgrade both of your package and billing cycle. See</mark> [<mark style="color:purple;">Upgrades and Downgrades</mark>](../../../pricing/general-lifecycle-rules.md#upgrades-and-downgrades) <mark style="color:blue;">for more details.</mark>
{% endhint %}

### 2. Select Access Method of Your End Users

* **Domain Name**: If your end users access your service via a domain name, (i.e., [www.zenlayer.com](http://www.zenlayer.com/)), please click on this button and enter the domain name in the field below.-- add dns record
* **IP Address**: If you want to accelerate a specific IP address or set of addresses, please make your selection(s) here.&#x20;

### 3. Provide Your Origin Information

Enter your origin address and choose a region closest to your origin.

### 4. Select Your Accelerator Type

* Standard (anycast)
* Custom Routing&#x20;

### 5. Set Your Acceleration Rules

Determine how traffic will be routed.

* HTTP and HTTPS
* TCP and UDP

### 6. Allocate to a Resource Group

Select a resource group for the accelerator so you can allocate resource groups to your team members.&#x20;



## What to Do Next

* If you selected Domain Name as the method your end users access your service in step **1.**, please be sure to add the CNAME provided by ZGA to your DNS record upon successful deployment of your accelerator. See [Add DNS Record](../add-dns-record.md)
* If you selected IP Address in step **1.**, please look into your accelerator details to get the accelerated IP address (virtual IP address) of each acceleration region (See [Manage Accelerator](../manage-accelerators.md)). Your end users can access your service directly by using the accelerated IP address.

