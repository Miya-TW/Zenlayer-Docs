---
description: >-
  After creating instances, you can search, modify, power off, power on, power
  cycle, and unsubscribe the instance.
---

# Manage Instances

## **Instance Information**

On the left menu bar, go to **Compute** > **Virtual Machine** > **Virtual Machine Instance**. Click the instance name or go to **Action** > **Details** to view CPU, bandwidth and configuration information of the instance. I’m&#x20;

### CPU and Bandwidth

* Click **Date** and select starting and ending time to view the CPU and bandwidth usage.
* Click **Power Off** on the upper right corner or select **Action** > **Power off** to power off the instance.
* Click **Power Cycle** on the upper right corner or select **Action** > **Power cycle** to power cycle the instance.

### Configuration Information

You can view basic configuration, storage, network, security group and billing information.

| Item                      | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><br>Configuration</p>  | <p><br>The basic configuration of the instance.<br>Click <strong>Change Password</strong> or go to <strong>Action</strong> > <strong>Change password</strong> to change the login password of your instance.</p><p><br><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;"><strong>Note</strong></mark><br><mark style="color:blue;">You can only change the password when the instance is powered off.</mark><br><mark style="color:blue;"></mark></p>                                                                                                                                                                                                          |
| <p><br>Storage</p>        | <p><br>Show the storage space of system disk and data disk.<br>Click <strong>View All Storage Information</strong> to view the virtual elastic disk list.<br></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| <p><br>Network</p>        | <p><br>Show instance public IPv4, private IPv4, network and subnet information.<br>Click the name of network and subnet to view details.<br></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| <p><br>Security Group</p> | <p><br>Show the security groups already deployed on the instance.</p><ul><li>Click the security group name to view details.</li><li>Click <strong>Undeploy</strong> to undeploy the security group.</li><li>Click <strong>Select Existing Security Groups</strong> to deploy existing security groups on the instance.</li><li>Click <strong>Create Security Group</strong> to create a new security group.</li></ul><p><strong></strong><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;"><strong>Note</strong></mark><br><mark style="color:blue;">You can deploy 2 security groups on one instance at most.</mark><br><mark style="color:blue;"></mark></p> |
| <p><br>Billing</p>        | <p><br>Show the created time, expiration time and billing information of the instance.<br>Click <strong>Unsubscribe</strong> or go to <strong>Action</strong> > <strong>Unsubscribe</strong> to cancel the instance subscription.<br></p><p><strong></strong><img src="../../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;"><strong>Note</strong></mark><br><mark style="color:blue;">You can resubscribe before expiration, or manually renew in 3 days after expiration. Otherwise, your data will be scrubbed 3 days after expiration.</mark><br></p>                                                                                                                    |



## **Network Information**

On the instance list interface, click VPC name in the **Network** column to view the information of network and subnet, as well as the instances attached.



## **Storage Information**

Click **Storage** in the **Configuration** column to view the disk list. You can also hover on <img src="../../../.gitbook/assets/1 (5).png" alt="" data-size="line"> to simply know about the size of different kind of disks.

