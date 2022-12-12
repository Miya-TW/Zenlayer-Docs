# Virtual Machine Instance

## Introduction

Virtual Machine Instance (VM Instance) is a subset of the Infrastructure as a Service (IaaS) cloud services bucket, providing high-performance, robust and scalable computing capability. You can deploy computing nodes globally in a convenient and flexible way by using Zenlayer virtual machine instances.\
\
A VM instance consists of CPU, memory, operating system, NIC, disks, etc. Users have full control over the instance. VM instance also includes function modules:

* **Virtual Elastic Disk**: a block storage service featured by high performance and low latency, providing distributed data disks for data storage. See Introduction to Virtual Elastic Disk for more information.
* **Security Group**: Security Group is a virtual firewall to control the inbound and outbound traffic of VM instance, in order to enhance the security. See Introduction to Security Group for more information.
* **VPC**: VPC (Virtual Private Cloud) is private network on Cloud and completely isolated. You can customize the private address range and divide subnets. See Introduction to VPC for more information.



## **Deployment Suggestions**

You are recommended to consider the following factors before creating VM Instance.

### **Location**

Location refers to Zenlayer's data center and determines the geolocation where your VM Instance is located. Once an instance has been successfully created, you will not be able to change the location. You can select the location based on factors such as users’ geolocation, availability of Zenlayer’s service, and application availability requirement. See the table later in this document to check the supported locations.

### **Network**

When creating VM Instance, you can customize the private network IP and subnets in order to highly isolate different systems, or private network & public network. See Network Planning for more details.

### Security

You can use Security Group free of charge to control the inbound and outbound policies of your instances as well as the port listening status. See Introduction to Security Group for more details.

_Note: The available models in each location vary depending on the inventory._

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">The available models in each location vary depending on the inventory.</mark>
{% endhint %}

****

## **Restrictions**

A single account (team) is permitted to create up to 999 VM instances. Please submit the support ticket or contact your sales representative to increase the limit.

### **Models**

|   Instance Model  | vCPU (Core) | RAM (GB) | Max. Bandwidth |
| :---------------: | :---------: | :------: | :------------: |
| Compute Optimized |      1      |     2    |       0.5      |
| Compute Optimized |      2      |     4    |        1       |
| Compute Optimized |      4      |     8    |       1.5      |
| Compute Optimized |      8      |    16    |        2       |
| Compute Optimized |      12     |    24    |       2.5      |
| Compute Optimized |      16     |    32    |        3       |
| Compute Optimized |      24     |    48    |       4.5      |
| Compute Optimized |      32     |    64    |        6       |
| Compute Optimized |      64     |    128   |        6       |
|  General Purpose  |      2      |     8    |        1       |
|  General Purpose  |      4      |    16    |       1.5      |
|  General Purpose  |      8      |    32    |        2       |
|  General Purpose  |      16     |    64    |        3       |
|  General Purpose  |      24     |    96    |       4.5      |
|  General Purpose  |      32     |    128   |        6       |
|  Memory Optimized |      2      |    16    |        1       |
|  Memory Optimized |      4      |    32    |       1.5      |
|  Memory Optimized |      8      |    64    |        2       |
|  Memory Optimized |      16     |    128   |        3       |

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">The available models in each location vary depending on the inventory.</mark>
{% endhint %}

### **Available Locations**

Virtual Machine instances are deployed by locations. Each location has its own power grid and network structure. Your instances in the same location can buildup private network by VPC.

| Location Code | City        |
| ------------- | ----------- |
| LAX           | Los Angeles |
| SIN           | Singapore   |

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">More locations will be added in the future.</mark>
{% endhint %}

### **Supported Operating System**

| OS      | Version              |
| ------- | -------------------- |
| CentOS  | centos 6.8 x86\_64   |
| CentOS  | centos 6.9 x86\_64   |
| CentOS  | centos 7.2 x86\_64   |
| CentOS  | centos 7.3 x86\_64   |
| CentOS  | centos 7.4 x86\_64   |
| CentOS  | centos 7.5 x86\_64   |
| CentOS  | centos 7.6 x86\_64   |
| CentOS  | centos 8.2 x86\_64   |
| Ubuntu  | ubuntu 14.04 x86\_64 |
| Ubuntu  | ubuntu 16.04 x86\_64 |
| Ubuntu  | ubuntu 18.04 x86\_64 |
| Ubuntu  | ubuntu 20.04 x86\_64 |
| Windows | windows 2008 x86\_64 |
| Windows | windows 2012 x86\_64 |
| Windows | windows 2016 x86\_64 |
| Windows | windows 2019 x86\_64 |

&#x20;
