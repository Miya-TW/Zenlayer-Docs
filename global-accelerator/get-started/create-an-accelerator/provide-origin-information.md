# Provide Origin Information

## **What is your origin address?**

Please enter the domain name or IP address of your origin site so ZGA can send user requests back to your origin site (**please note**: one accelerator can only accelerate one origin site, therefore only one domain name can be entered here; multiple IPs can be entered as long as all of them belong to the same origin site). You can also select a result from the Origin Address lookup.

_**\*Domain Name (entered in the first step) and Origin Domain Name**:_ \
_The domain name you entered in the first step is used for end-user access. The origin domain name is used by ZGA to send user requests back to your origin site. Please make sure the **origin domain name** you entered is different from the **domain name**. If you use a public cloud provider, you should be able to find your origin domain name or IP address in your provider's console. If you can’t find either one, please consult with your operations personnel._

_**\*Origin Address lookup**_\
_In order to continue your setup, once you’ve entered the domain name for user access, the console will automatically look up the IP and domain name of the corresponding origin server._

_**\*Under what circumstances would your origin domain name not match your domain name?**_

* _If you use a public cloud load balancing service (such as AWS's ELB), your origin will be delivered with a domain name_
* _Your origin site is configured with multiple IPs, and these IPs all point to the same origin domain name. When an IP encounters an issue, the origin domain name will resolve to other functioning IPs to maintain high availability_

## **Where is your origin located?**

Select the region where your origin site is located from the drop-down menu. If that region is not on the list, select the next closest region to your origin site.

_If your origin is in Mainland China and end users access your service by domain name, please ensure that you have a corresponding Chinese ICP license number._
