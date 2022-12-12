# Add DNS Record

\
If end users access your service through domain name, please use your provider’s platform to add the CNAME provided by your Zenlayer Global Accelerator (ZGA) to your DNS record upon successful deployment.

#### **1. CNAME Record (Recommended)**

\
After a successful deployment, ZGA will assign your accelerator a CNAME that can be found in the accelerator list (see [Manage Accelerator](manage-accelerators.md)). You will need to add the CNAME record into your DNS so that your domain name can be resolved to your ZGA’s CNAME in your acceleration regions.

_**\*About CNAME**_\
_A CNAME (canonical name) is a type of resource record in the DNS (domain name system) that maps one domain name (an alias) to another (the canonical name). This can prove convenient when running multiple services (like an FTP server and a web server, each running on different ports) from a single IP address. One can, for example, point_ [_ftp.example.com_](https://zenlayer.lightning.force.com/lightning/r/Knowledge\_\_kav/ka06S0000015JcVQAU/ftp.example.com) _and www.example.com to the DNS entry for_ [_example.com_](http://example.com/)_, which in turn has a record which points to the IP address. (From Wikipedia)_

Follow the guides listed below to add a CNAME record to your DNS.\
&#x20;

\
If you use another DNS provider, please reach out to them directly for instructions on how to add a CNAME record.\
&#x20;

#### **2. A Record (address record)**

_\*If you have added a CNAME record, there is no need to add an A record. We recommend that you add a CNAME record._

After a successful deployment, ZGA will assign each of your acceleration regions a VIP (virtual IP) that can be found in the accelerator list (see [Manage Accelerator](manage-accelerators.md)).  You can add an A record to your DNS so that your domain name will be resolved to the ZGA IP in each acceleration region.

Follow the guides listed in the **CNAME record** section above to add an A record to your DNS.

_\*Since each VIP is assigned to an acceleration region, please add a separate A record for each region. (Some DNS providers may not support specifying geo-locations. In this case, an A record is not recommended, and you will need to add a CNAME record instead.)_

Your accelerator will start routing traffic after your DNS record has been updated.
