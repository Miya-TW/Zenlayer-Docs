# Concepts

## **OnRamp (First Mile)**

### **Cloud Connect**

A connection between Zenlayer’s backbone network and a public cloud that has been established offline. You can select the cloud connect closest to your infrastructure on the public cloud.

****

## **Access (Last Mile)**

A connection between the data center or the office and Zenlayer’s backbone network.

### **Port**

A port is a physical access point of equipment in SDN backbone POPs (points of presence) at which two or more networks or communication devices share a connection to an ISP (Internet service provider).

Your data center and office need to be connected to the port to transmit data.

### **Cross Connect**

The hardware, such as cables, cords, and jumpers, that connect separate units of the facilities. A cross-connection can be viewed as a direct physical point-to-point connection running from one server to another.

If your data center is close enough to the port to be connected, you can use cross connect with physical cables.

### **Local Loop**

A wired connection that connects your office or data center to the nearest equipment port in our SDN POPs. The wiring used in the local loop is usually UTP (unshielded twisted pair) cabling, and the transmission method is analog transmission.&#x20;

If there is a short distance between your office or data center and the port to be connected, you can use a local loop to connect them.

### **Virtual Edge**

A cost-effective solution to ensure VPN (virtual private network) service isolation and security. Traditional BGP/MPLS (border gateway protocol/multiprotocol label switching) IP VPN technology requires a CE (customer edge) to be deployed for each VPN to connect to upper-layer devices. This drives up costs and complicates deployment. Virtual edge, by contrast, provides an economical and easy-to-manage solution.

When you need a Layer 3 network connection and there is a large distance between your office and the equipment port in our SDN POPs, you can create an IPsec (Internet protocol security) tunnel from your office to the virtual edge to quickly connect to Zenlayer backbone at a lower cost.&#x20;

****

## **Fabric (Backbone Network)**

### **Private Connect**

A Layer 2 (or data-link layer) network connection based on our SDN backbone network, consisting of two end nodes connected by a leased line. A protocol over the WAN (wide-area network) link encapsulates local network traffic into frames for transmission.

<figure><img src="https://support.zenlayer.com/servlet/rtaImage?eid=ka06S000001Lw6D&#x26;feoid=00N3h00000EQw1z&#x26;refid=0EM6S000003ZNsX" alt=""><figcaption><p><strong>Private Connect</strong></p></figcaption></figure>

### **Cloud Router**

A Layer 3 network connection based on our SDN backbone network consisting of multiple end nodes. Cloud router groups and routes traffic from dozens or even hundreds of physical LAN (local area network) segments to maintain high performance and reliability.

<figure><img src="https://support.zenlayer.com/servlet/rtaImage?eid=ka06S000001Lw6D&#x26;feoid=00N3h00000EQw1z&#x26;refid=0EM6S000003ZNsc" alt=""><figcaption><p>Cloud Router</p></figcaption></figure>

