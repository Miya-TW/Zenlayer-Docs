# Public Virtual Interface

## **What is a public virtual interface?**

Zenlayer public virtual interfaces are a VLAN/VXLAN based technology to group your instances' public network interfaces, which provides a partitioned and isolated network zone at the data link layer (OSI layer 2). The bare metal instances attached to same Public Virtual Interface can communicate with each other via ethernet layer-2 protocol (e.g., ARP).

Public virtual interfaces are supported in all Zenlayer bare metal cloud zones, excepts for Los Angeles Zone B and Frankfurt Zone A.\
Public virtual interfaces are zone-specific resources and can only work with bare metal instances within the same zone.



## **Features**

There are several benefits to adding a public virtual interface to your infrastructure:

* Isolated and secured network segment
* Floating IP between different instances

Use a Public Virtual Interface if you want to:

* Build your own LVS in DR mode
* Float IP address between instances for application requirement or redundancy
* Get a bigger IP range and start using it immediately
* Attach more instances for the same IP range in future

****

## **Limits**

* Public virtual interfaces do not support IPv6.
* Public virtual interfaces use CIDR notation to represent the IP space.\
  For example, a /29 represents a 29 leading 1-bits subnet mask (255.255.255.248), an IP space with 8 IP addresses. Take out the network ID and broadcast IP, and we will use the first usable IP for your VLAN gateway, then you will get 8-3=5 usable IP addresses.
* When you attach the instances to the public virtual interfaces, you will be asked to pick up one usable IP for the instance, and the instance's existing internet IP address will be replaced by the public virtual interfaces' usable IP address.

## **Public Virtual Interface VS Elastic IP**

* Public virtual interface provides Layer 2 communication between servers, and most of the technologies such as load balancing, redundancy DR and IP floating are based on Layer 2 communication. Therefore if you need to deploy the above technologies, please create a public virtual interface first.
* Elastic IP only provides additional public IP, and one IP can only be used for one server at the same time. In addition an elastic IP does not support Layer 2 communication with other IPs.

## **Public Virtual Interface VS Virtual Private Cloud**

Public virtual interface provides public Layer 2 communication while Virtual Private Cloud provides private Layer 2 communication.

* If your business requires public communication between servers on the same zone, please create a public virtual interface.
* Functions like load balancing, firewall and DDoS protection need to be built upon public Layer 2 communication.

