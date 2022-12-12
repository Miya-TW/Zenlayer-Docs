# VPC & Subnet Planning

Before you create VPC and subnet, you should plan the number of VPC and subnet, and CIDR blocks of VPC and subnet.



## **Number of VPCs**

If you do not need to deploy your applications across locations or isolate service systems, we recommend that you create only one VPC.\
We recommend that you create multiple VPCs if you have one of the following requirements:

* Cross-location deployment\
  A VPC cannot be deployed across locations. Therefore, if you want to deploy your application systems in different locations, you must create multiple VPCs. \
  You can use Cloud Networking to connect VPCs that are deployed in different locations.\
  \
  <img src="../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;">**Note**</mark>\ <mark style="color:blue;">****</mark><mark style="color:blue;">This feature is not available on zenConsole at present, please contact our sales or raise support ticket.</mark>\ <mark style="color:blue;"></mark>
* Service isolation\
  If you want to isolate your service systems in the same location by using VPC, you must create multiple VPCs. \
  For example, you can use multiple VPCs to isolate the test environment from the production environment.



## **Number of Subnets**

You can determine the number of subnets based on the following suggestions:

* Create at least two subnets for each VPC to implement disaster recovery.\
  Network latency between different subnets in the same VPC is typically low. However, you must check the actual network latency after you deploy your services. The network latency may be increased due to the complex network topology. \
  We recommend that you optimize and adapt the system to meet your requirements for high availability and low latency.\

* Consider the scale and planning of your service system.\
  If you want the frontend system to communicate with the Internet, we recommend that you deploy different frontend systems in different subnets and deploy backend systems in other subnets. This improves service availability.



## **CIDR Block**

When you create VPCs and subnets, you must specify their private IP address ranges in CIDR notation.&#x20;

### **VPC CIDR blocks**

You can specify 192.168.0.0/16, 172.16.0.0/12, 10.0.0.0/8, or one of their subnets as the CIDR block of a VPC. When you specify CIDR blocks for VPCs, please note:

* If you have only one VPC and the VPC does not need to communicate with a data center, you can specify one of the CIDR blocks or their subsets listed above as the VPC CIDR block.\

* If you have multiple VPCs or want to set up a hybrid cloud environment between a VPC and your data center, we recommend that you specify the subsets of the above CIDR blocks for your VPCs. In this case, we recommend that you set the subnet mask length to 16 bits or less. Make sure that the CIDR blocks of the VPCs and your data center do not overlap.

### **Subnet CIDR blocks**

The CIDR block of a subnet must be a subset of the CIDR block of the VPC to which the subnet belongs. For example, if the CIDR block of a VPC is 192.168.0.0/16, the CDIR block of a subnet that belongs to the VPC can range from 192.168.0.0/17 to 192.168.0.0/29. When you specify CIDR blocks for subnets, please note:

* The subnet mask of a subnet must be 17 to 29 bits in length, which provides 8 to 65,536 IP addresses.\

* The first two and last one IP addresses of each subnet CIDR block are reserved. For example, if the CIDR block of a subnet is 192.168.1.0/24, IP addresses 192.168.1.0, 192.168.1.1, and 192.168.1.255 are reserved.\

* Consider the number of VM instances that you want to deploy in a subnet before you specify a CIDR block for the subnet.



## **A Scenario: Connecting a VPC to Another VPC or a Data Center**

If you want to connect a VPC to another VPC or a data center, make sure that the CIDR blocks do not overlap with each other. Also note:

* We recommend that you specify different CIDR blocks for different VPCs.\

* If you cannot specify different CIDR blocks for different VPCs, try to specify different CIDR blocks for subnets that belong to different VPCs.\

* If neither of the preceding requirements is met, make sure that the CIDR blocks of subnets that need to communicate with each other are different.

