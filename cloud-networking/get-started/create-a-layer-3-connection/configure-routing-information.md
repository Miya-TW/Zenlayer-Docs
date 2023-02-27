---
description: >-
  If you add access points like data centers or public clouds, you need to
  configure routing protocols to achieve network communication.
---

# Configure Routing Information

## Prerequisites

* If you add a VPC, you don't need to configure the routing information. Go to [Network Configuration](configure-network-information.md) directly.
* If you have a small network, you can choose static routing. If you have a big network and your devices support Border Gateway Protocol (BGP), we recommend using BGP to take care of network segment changes.

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption><p>Routing Configuration</p></figcaption></figure>

## BGP Routing

BGP (border gateway protocol) is usually used to maintain complex networks that contain many routers. BGP divides an intranet into groups of routers, or AS (automated systems), which have trusted routes between them. You must define the AS number on the routers in your network and configure at least one group that includes at least one peer. BGP supports MD5 (message-digest algorithm 5) to secure messages.

## Static Routing

Static routing is generally used in smaller networks that contain only a couple of routers, or when security is an issue. Each static router must be configured and maintained separately.



* **Your intranet address**: the private IP configured on your data center/public cloud access point.
* **Zenlayer intranet address**: the private IP configured on Zenlayer backbone POP.
* **Your ASN**: the ASN of your data center/public cloud access point. Only available for BGP configuration.
* **Zenlayer ASN**: 62610 by default and cannot be changed. Only available for BGP configuration.
* **BGP MD5 of customer**: BGP authentication key.Only available for BGP configuration.

