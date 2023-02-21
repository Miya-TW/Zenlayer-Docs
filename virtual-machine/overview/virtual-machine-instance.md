# Virtual Machine Instance

## Introduction

Virtual Machine Instance (VM Instance) is a subset of the Infrastructure as a Service (IaaS) cloud services bucket, providing high-performance, robust and scalable computing capability. You can deploy computing nodes globally in a convenient and flexible way by using Zenlayer virtual machine instances.\
\
A VM instance consists of CPU, memory, operating system, NIC, disks, etc. Users have full control over the instance. VM instance also includes function modules:

* **Virtual Elastic Disk**: a block storage service featured by high performance and low latency, providing distributed data disks for data storage. See Introduction to [Virtual Elastic Disk](virtual-elastic-disk.md) for more information.
* **Security Group**: Security Group is a virtual firewall to control the inbound and outbound traffic of VM instance, in order to enhance the security. See Introduction to [Security Group](security-group.md) for more information.
* **VPC**: VPC (Virtual Private Cloud) is private network on Cloud and completely isolated. You can customize the private address range and divide subnets. See Introduction to [VPC](vpc.md) for more information.



## **Deployment Suggestions**

You are recommended to consider the following factors before creating VM Instance.

### **Location**

Location refers to Zenlayer's data center and determines the geolocation where your VM Instance is located. Once an instance has been successfully created, you will not be able to change the location. You can select the location based on factors such as users’ geolocation, availability of Zenlayer’s service, and application availability requirement. See [Available Locations](models-zones-and-operating-system.md#available-locations) to check the supported locations.

### **Network**

When creating VM Instance, you can customize the private network IP and subnets in order to highly isolate different systems, or private network & public network. See [VPC & Subnet Planning](vpc-and-subnet-planning.md) for more details.

### Security

You can use Security Group free of charge to control the inbound and outbound policies of your instances as well as the port listening status. See Introduction to [Security Group](security-group.md) for more details.

_Note: The available models in each location vary depending on the inventory._

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">The available models in each location vary depending on the inventory.</mark>
{% endhint %}

****

## **Restrictions**

A single account (team) is permitted to create up to 999 VM instances. Please submit the support ticket or contact your sales representative to increase the limit.

