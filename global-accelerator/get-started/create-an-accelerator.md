# Create an Accelerator

After logging in to Console, click on **Create an Accelerator** on the homepage. You will first need to select your acceleration package by clicking on **Create Global Accelerator**.

Note:

* If this is your first time creating an accelerator, you can try out the Basic Package for 7 days for free.
* You can upgrade to a paid subscription package before your trial expires.

\
After you’ve selected your package, follow these to create your accelerator:\
&#x20;\
**1. What would you like to accelerate?**

Select the method end users access your service from the two options shown:

* **Domain Name**: If your end users access your service via a domain name, (i.e., [www.zenlayer.com](http://www.zenlayer.com/)), please click on this button and enter the domain name in the field below.
* **IP Address**: If you want to accelerate a specific IP address or set of addresses, please make your selection(s) here.&#x20;

_\*If you are not sure whether you should select Domain Name or IP, please consult your operations personnel._

Regardless of your selection above, we will provide you with the IP and CNAME of your ZGA (Zenlayer Global Accelerator) upon successful completion of your deployment. See [Manage Accelerator](manage-accelerators.md).

* **Domain name**: Please be sure to add the CNAME to your DNS record. See [Add DNS Record](add-dns-record.md)
* **IP Address**: Directly use the IP address provided by ZGA for user access

&#x20;\
**2. What is your origin address?**

Please enter the domain name or IP address of your origin site so ZGA can send user requests back to your origin site (**please note**: one accelerator can only accelerate one origin site, therefore only one domain name can be entered here; multiple IPs can be entered as long as all of them belong to the same origin site). You can also select a result from the Origin Address lookup.

_**\*Domain Name (entered in the first step) and Origin Domain Name**:_ \
_The domain name you entered in the first step is used for end-user access. The origin domain name is used by ZGA to send user requests back to your origin site. Please make sure the **origin domain name** you entered is different from the **domain name**. If you use a public cloud provider, you should be able to find your origin domain name or IP address in your provider's console. If you can’t find either one, please consult with your operations personnel._

_**\*Origin Address lookup**_\
_In order to continue your setup, once you’ve entered the domain name for user access, the console will automatically look up the IP and domain name of the corresponding origin server._

_**\*Under what circumstances would your origin domain name not match your domain name?**_

* _If you use a public cloud load balancing service (such as AWS's ELB), your origin will be delivered with a domain name_
* _Your origin site is configured with multiple IPs, and these IPs all point to the same origin domain name. When an IP encounters an issue, the origin domain name will resolve to other functioning IPs to maintain high availability_

**3. Where is your origin located?**

Select the region where your origin site is located from the drop-down menu. If that region is not on the list, select the next closest region to your origin site.

_If your origin is in Mainland China and end users access your service by domain name, please ensure that you have a corresponding Chinese ICP license number._

\
**4. Which regions would you like to accelerate?**

Select all the regions you want to accelerate. An acceleration line will be generated between your selected origin and each acceleration region.\
**5. Set your acceleration rules**

Tell us the protocol and port used by your service so that ZGA can forward user requests correctly:

**HTTP and HTTPS**: The default ports are 80 and 443 (can be modified); if you choose HTTPS, you will need to upload the necessary key and certification.\
**TCP and UDP**: The default ports are 80 and 53 (can be modified).\
If you selected IP Address in step **1**. above as the user access method, only TCP and UDP will be available here.

\
**6. Add resource group**

Select a resource group for the accelerator so you can allocate resource groups to your team members.  \
&#x20;\
**7. Price details**

Confirm the pricing and details of your selected package, then click **Create Now!** to complete payment and start your subscription.

_\*Learn more about ZGA's Pricing rules in_&#x20;

[ZGA Pricing](../../pricing/global-accelerator-pricing.md)

Once the payment is completed, your accelerator will be deployed in a few minutes.

**Important!**

* If you selected Domain Name as the method your end users access your service in step **1.**, please be sure to add the CNAME provided by ZGA to your DNS record upon successful deployment of your accelerator. See [Add DNS Record](add-dns-record.md)
* If you selected IP Address in step **1.**, please look into your accelerator details to get the accelerated IP address (virtual IP address) of each acceleration region (See [Manage Accelerator](manage-accelerators.md)). Your end users can access your service directly by using the accelerated IP address.
