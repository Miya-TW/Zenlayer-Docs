# Manage Accelerators

#### &#x20;**1. Accelerator List**

\
After your accelerators are deployed successfully, you can view them in this list and access the following:&#x20;

_The indicator on the left shows the status of each accelerator:_\
_**Spinning circle**: Deployment in process_\
_**Green**: Accelerator is active_ \
_**Gray**: Accelerator is paused_\
_**Red**: Deleted_

* **Search**

Search for specific accelerators by selected conditions

&#x20;

* **CNAME**

Here you will see the CNAME for each accelerator provided by your Zenlayer Global Accelerator (ZGA). If your end users access your service by domain name, you will need to add the CNAME record to your DNS so that your domain name can be resolved to your ZGA’s CNAME in your acceleration regions.\
Refer to [Add DNS Record](add-dns-record.md) for more information

&#x20;

* **Actions**

Click on **Actions** on the right to access the following: \
**Details**: Check the details of your accelerator. See [Accelerator Details](manage-accelerators.md#2.-accelerator-details)\
**Pause**: Pause your accelerator. After acceleration is paused, data transfer will no longer incur any fees, but the cost to maintain your accelerator will still be billed normally.\
**Delete**: Delete your accelerator. Your configuration data will be retained for 7 days and can be recovered by clicking on **Recover**. Please note that your data will be permanently deleted after 7 days. You can also click on **Destroy** to immediately delete your data.\
&#x20;

#### **2. Accelerator Details**

\
Click on the name of any of your accelerators to view the following:\
&#x20;

* **Usage Graph**

This page shows the bandwidth and data usage of your selected accelerator. You can set the time range, acceleration region, and acceleration rule to alter how your usage is graphed.\
&#x20;\
_\*Bandwidth: The rate at which data is transmitted. Hover your mouse over the chart to see the value of incoming and outgoing bandwidth at each time point._\
_\*Data Transfer: The amount of data transferred. Hover your mouse over the chart to view the amount of inbound and outbound traffic at each time point._&#x20;

* **Update Accelerator Configuration**

This page displays the configuration information of your accelerator and lets you access the following: \
&#x20;

| **Update origin domain name or IP address** | Modify the domain name or IP of the origin site. Refer to [Create Accelerator](broken-reference) to learn more.                                                                                                                                                                                                                                                                                                                               |
| ------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **CNAME**                                   | Refer to [Add DNS Record](add-dns-record.md)                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Update Acceleration Regions**             | Modify the acceleration region. Refer to [Create Accelerator](broken-reference) to learn more.                                                                                                                                                                                                                                                                                                                                                |
| **VIP of each acceleration region**         | <p>VIP (virtual IP) is the accelerated IP assigned to your accelerator for each region. You can use the VIP to:</p><ul><li>Give your end users direct access in the corresponding regions if they access your service by IP address </li><li>Resolve your domain name by adding A record (address record) to your DNS if your end users access your service through domain name. See <a href="add-dns-record.md">Add DNS Record</a></li></ul> |
| **Update Acceleration Rules**               | You can modify the protocol and port of your accelerator here, then click on **Update** **Acceleration Rules** to confirm your changes. To restore these parameters to the default setting, click on **Reset**.                                                                                                                                                                                                                               |

&#x20;

* **Access Management**

If you want to control user access, click on **Set** **Access Limits** and enable whitelist or blacklist as needed:

_\*Whitelist: Enter the end user IPs that you wish to allow access to your service_\
_\*Blacklist: Enter the end user IPs that you wish to block access to your service_\
&#x20;\
Click on **Change access limits** to confirm your changes. To restore these parameters to the default setting, click on **Reset** &#x20;

* **Delete Accelerator**

Upon deletion, your configuration data will be retained for 7 days and can be recovered by clicking on **Recover**. Please note that your data will be permanently deleted after 7 days. You can also click on **Destroy** to immediately delete your data.\
&#x20;
