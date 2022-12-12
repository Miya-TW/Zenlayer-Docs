# Elastic IP

## **What is an elastic IP?**

Each bare metal instance is originally assigned with a piece of public IP address when you open it. \
Elastic IPs are also publicly accessible static IP addresses that you can assign to bare metal instance. You can remap them among instances in the same zone to move the application to another instance or assign more than one Elastic IP to an instance for applications requiring multiple IP addresses.\
Elastic IPs with function of DDoS protection are called DDoS protected elastic IPs, which help you to scrub malicious traffic so as to prevent network attacks.\
Elastic IPs are available in all zones. They are zone-specific resources and can only be assigned to bare metal instances within the same zone.

****

## **Features**

* Assigning an elastic IP to an instance doesn't replace or change its original public IP address. Elastic IPs will be assigned as secondary IP to the internet facing network interface of bare metal instance.
* You can use elastic IPs to create instance infrastructures without single points of failure, but an elastic IP alone does not provide failover automatically. In case of active instance failures with the elastic IP assigned, you can unbind it and reassign it to a standby instance to redirect network traffic.

****

## **Limits**

* You cannot assign an elastic IP to more than one instance at a time.
* Elastic IPv6 is not supported. All elastic IPs are IPv4.
* A bare metal instance must keep original IP active to ensure accessibility of corresponding elastic IPs.

