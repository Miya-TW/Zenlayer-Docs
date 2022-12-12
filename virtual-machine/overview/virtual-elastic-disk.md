# Virtual Elastic Disk

Virtual Elastic Disk is elastic block storage service provided by Zenlayer for Virtual Machine Instances and provides low latency, high performance, high durability, and high reliability. Virtual Elastic Disk uses a distributed triplicate mechanism to copy your data within the location to ensure data durability and availability.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">The information about Virtual Elastic Disk in this document is applicable to the data disk created together with the VM instance.</mark>
{% endhint %}



## **Virtual Elastic Disk Limits**

A disk can be attached only to a single VM instance in the same location.

| Item                                                   | Limits                                                          |
| ------------------------------------------------------ | --------------------------------------------------------------- |
| Maximum number of Virtual Elastic Disks on an instance | 10 (including the data disk created together with the instance) |
| Capacity of a single Virtual Elastic Disk (GB)         | 20 - 2000                                                       |

