# VLAN

## **What is a** VLAN**?**

Zenlayer VLANs are a VLAN/VXLAN based technology to group your instances' public network interfaces, which provides a partitioned and isolated network zone at the data link layer (OSI layer 2). The bare metal instances attached to same VLAN can communicate with each other via ethernet layer-2 protocol (e.g., ARP).

VLANs are supported in all Zenlayer bare metal cloud zones, excepts for Los Angeles Zone B and Frankfurt Zone A.\
VLANs are zone-specific resources and can only work with bare metal instances within the same zone.



## **Features**

There are several benefits to adding a VLAN to your infrastructure:

* Isolated and secured network segment
* Floating IP between different instances

Use a VLAN if you want to:

* Build your own LVS in DR mode
* Float IP address between instances for application requirement or redundancy
* Get a bigger IP range and start using it immediately
* Attach more instances for the same IP range in future

****

## **Limits**

* VLANs do not support IPv6.
* VLANs use CIDR notation to represent the IP space.\
  For example, a /29 represents a 29 leading 1-bits subnet mask (255.255.255.248), an IP space with 8 IP addresses. Take out the network ID and broadcast IP, and we will use the first usable IP for your VLAN gateway, then you will get 8-3=5 usable IP addresses.
* When you attach the instances to the VLANs, you will be asked to pick up one usable IP for the instance, and the instance's existing internet IP address will be replaced by the VLANs' usable IP address.

## VLAN **VS Elastic IP**

* VLAN provides Layer 2 communication between servers, and most of the technologies such as load balancing, redundancy DR and IP floating are based on Layer 2 communication. Therefore if you need to deploy the above technologies, please create a VLAN first.
* Elastic IP only provides additional public IP, and one IP can only be used for one server at the same time. In addition an elastic IP does not support Layer 2 communication with other IPs.

## VLAN **VS Virtual Private Cloud**

VLAN provides public Layer 2 communication while Virtual Private Cloud provides private Layer 2 communication.

* If your business requires public communication between servers on the same zone, please create a VLAN.
* Functions like load balancing, firewall and DDoS protection need to be built upon public Layer 2 communication.

