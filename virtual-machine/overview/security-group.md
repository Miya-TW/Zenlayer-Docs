# Security Group

Security Group acts as virtual firewall to control the inbound and outbound traffic of Virtual Machine Instance to improve security. Security Group provides Stateful Packet Inspection (SPI) and packet filtering capabilities. You can use security group and its rules to define security domains in the Cloud.

## **Limits**

| Item                                                                        | Limits           |
| --------------------------------------------------------------------------- | ---------------- |
| Maximum number of security groups                                           | 2                |
| Maximum number of security groups that can be deployed on a single instance | 2                |
| Maximum number of rules in a security group                                 | <p>400 <br> </p> |



## **Practical suggestions**

* If you don't create security group, the system applies to your instances a default security group which only allows inbound connections to port 22 (Linux) and 3389 (Windows) for remote log in.\

* You can add rules to allow access to or from specific destinations or sources on specific ports.\

* Follow the principle of least authorization when you add security group rules. For example, to allow connections to port 22 on a Linux instance, we recommend that you add a rule to allow access from only specific IP addresses instead of all IP addresses (0.0.0.0/0).\

* Make sure that each security group has simple and clear rules. A single instance can be added to multiple security groups. A single security group can have multiple rules. If a large number of rules are applied to an instance, management is complex and unforeseen risks can be introduced.\

* Add instances that serve different purposes to different security groups and separately maintain the security group rules applied to the instances. For example, you can add instances that accept the Internet access to a security group. Then, in this security group, add rules to allow inbound access to only the ports used to provide external services, such as ports 80 and 443. Meanwhile, to ensure that the instances accessible from the Internet do not provide other services (such as MySQL and Redis), we recommend that you deploy internal services on the instances inaccessible from the Internet and add these instances to another security group.\

* Do not modify security groups used in the production environment. All changes to a security group are automatically applied to the instances within the security group. Before you change a security group, you can clone, change, and debug it within the test environment to ensure that the change does not interrupt the communication between the associated instances.\

* Specify identifiable names and descriptions for security groups for easy search and management.

