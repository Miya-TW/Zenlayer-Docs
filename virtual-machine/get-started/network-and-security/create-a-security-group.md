---
description: >-
  You can set your security group rules for your instances on zenConsole to
  improve the network security. The security group applies to both public and
  private network access to your instances.
---

# Create a Security Group

## Procedures

### Step 1 - Sign in and go to create

1. Log in to [**zenConsole**](https://console.zenlayer.com/).
2. Go to **Compute** > **Virtual Machine** > **Security Group** and click **Create Security Group**.



### Step 2 - Identify your security group



### Step 3 - Configure the inbound and outbound rules

| Item                          | Description                                                                                                                                                                             |
| ----------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Type                          | **Accept**：allows access requests on a specific port.                                                                                                                                   |
| Priority                      | <p>A smaller value indicates a higher priority.<br><strong>Valid values</strong>: 1 to 100.</p>                                                                                         |
| Protocol                      | <p>The protocol type of the security group rule. <br><strong>Valid values</strong>: All/TCP/UDP/All ICMP (IPv4)</p>                                                                     |
| Port range                    | You can specify a port range when **Protocol Type** is set as **TCP** or **UDP**. Enter one or more port ranges. Separate the port ranges with commas (,). **Example**: 22/23, 443/443. |
| <p>Source/<br>Destination</p> | <p>Configure the host IP addresses of source and destination.<br><strong>Example</strong>: 192.168.0.0/24. 0.0.0.0/0 or ::/0 indicates all IP addresses are allowed.</p>                |
| Actions                       | Delete the rule.                                                                                                                                                                        |



Typical applications of commonly used ports are shown as follows:

| Scenario                                       | Rule direction | Authorization policy | Protocol type | Port range | Authorization type                            | Authorization object                                   | Priority |
| ---------------------------------------------- | -------------- | -------------------- | ------------- | ---------- | --------------------------------------------- | ------------------------------------------------------ | -------- |
| Remote access to Linux instances through SSH   | Inbound        | Allow                | SSH (22)      | 22/22      | Address field access                          | 0.0.0.0/0                                              | 1        |
| Remote access to Windows instances through RDP | Inbound        | Allow                | RDP (3389)    | 3389/3389  | Address field access                          | 0.0.0.0/0                                              | 1        |
| Ping VM instances through the Internet         | Inbound        | Allow                | ICMP          | -1/-1      | Address field access or security group access | Set this parameter according to the authorization type | 1        |
| Use a VM instance as a Web server              | Inbound        | Allow                | HTTP (80)     | 80/80      | Address field access                          | 0.0.0.0/0                                              | 1        |
| Upload or download files through FTP           | Inbound        | Allow                | Custom TCP    | 20/21      | Address field access                          | 0.0.0.0/0                                              | 1        |



### Step 4 - Select an instance to apply the security group to



### Step 5 - _<mark style="color:green;">(Optional)</mark>_ describe the security group



### Step 6 - Click _**Create**_ to create a security group



### Step 7 - Manage security groups

* Deploy the security group\
  On the security group interface, click the instances deployed the security group on to change or add the instance.\

* Edit the security group\
  On the security group interface, click **Edit** to change inbound and outbound rules.\

* Delete the security group\
  On the security group interface, click **Delete** to delete the security group then the instance will not be controlled by the rules.

