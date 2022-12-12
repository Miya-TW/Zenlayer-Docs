# VPC

A Virtual Private Cloud (VPC) is your dedicated private network on Zenlayer Cloud. You have full control over your VPC. For example, you can specify the CIDR block and divide subnets. Virtual Machine Instances will be managed under the VPC.



## **Components**

Each VPC consists of at least one private CIDR block and at least one Subnet.

### **Private CIDR Block**

When you create VPC and Subnet, you must specify the private IP address range for the VPC in CIDR notation.

You can use one of the standard private CIDR blocks listed in the following table or their subnets as the private CIDR block of a VPC. For more information, see Network Planning.

| Private CIDR Block | Number of Available Private IP Addresses                              |
| ------------------ | --------------------------------------------------------------------- |
| 192.168.0.0/16     | <p>65,532 (excluding IP addresses reserved<br>by the system)</p>      |
| 172.16.0.0/12      | <p>1,048,572  (excluding IP addresses reserved<br>by the system)</p>  |
| 10.0.0.0/8         | <p>16,777,212  (excluding IP addresses reserved<br>by the system)</p> |

### **Subnet**

A Subnet is a basic network component. After creating a VPC, you can create subnets to divide the VPC into one or more subnets. Subnets deployed in a VPC can communicate with each other over the private network. You can deploy your applications in different subnets to improve service availability.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">You cannot directly deploy VM instances in a VPC. You must deploy them in subnets of a VPC.</mark>
{% endhint %}



## **Application Scenarios**

VPCs are virtual networks that are fully isolated from each other. VPCs support flexible configurations to meet requirements of different scenarios.

#### **Deploy applications in a safe manner**

You can deploy applications which provide external services in the VPC, and create security group to control access from the Internet. You can also isolate application servers from database by deploying web servers in a subnet that can access the Internet, and deploying database in another subnet that cannot access the Internet.

#### **Isolate business systems**

VPCs are logically isolated from each other. You can use multiple VPCs to isolate business systems in different environments such as production and test environments. If you want to enable a VPC to communicate with another one, you can attach the VPCs to Cloud Networking.&#x20;

For more information, please contact Zenlayer Sales or submit support ticket on zenConsole.

#### **Build a hybrid cloud**

To expand your on-premises network, you can establish a dedicated connection between a VPC and your data center. This allows you to seamlessly migrate the applications in your data center to the cloud. You do not need to change the access method for the applications.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">If you need dedicated connection between VPCs, or between VPC and on-premises data center, please raise support ticket on zenConsole, or contact Zenlayer Sales.</mark>
{% endhint %}



## **Limits**

| Item                                                | Limits                                                                          |
| --------------------------------------------------- | ------------------------------------------------------------------------------- |
| Number of VPCs that can be created in each location | 2                                                                               |
| Number of subnets that can be created in each VPC   | 3                                                                               |
| Available CIDR blocks for each VPC                  | <p>10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16, or one of their subnets.<br> </p> |

