---
description: >-
  Bare metal instances, bandwidth, data transfer, elastic IPs, CIDR blocks are
  billable; virtual private clouds (VPCs) and subnets are free for use.
---

# Billing Method

## Bare Metal Instance

*   Hardware configurations:

    Operating systems; HDD/SAS/SATA; RAID; etc.
* A piece of public IPv4
* A piece of public IPv6 (subject to zones)
* Included bandwidth (10 M/30 M/50 M/100 M subject to zones)

You prepay the instance by month in each subscription period. The longer the billing cycle, the bigger the discount.



## Bandwidth

### Flat Rate Bandwidth

You can set a bandwidth cap for your stable business with little bursty traffic, and use unlimited data transfer. You will be charged based on the bandwidth size.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">You can postpay your bandwidth together with the instance by hour.</mark>

<mark style="color:blue;">Please contact us if you need.</mark>
{% endhint %}

### Burstable 95th

You use first and pay afterward by month. If you have a base commit rate, you need to pre-pay that part first. The system samples the peak bandwidth of each instance monthly, and discard the top 5% of the samples. The highest value left is taken as your actual bandwidth usage. Instances with pricing model of burstable 95th will be billed as follows:

Monthly payment = Resource payment (Monthly price of computing + storage) + Bandwidth payment (95th percentile bandwidth (Mbps) × Monthly price per Mbps × Effective factor).

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">Effective factor = Number of valid days in a calendar month/Total number of days in the calendar month.</mark>
{% endhint %}

There are 3 kinds of burstable 95th billing models:

<table><thead><tr><th>Billing Model</th><th>Billing Item</th><th>Description</th><th data-hidden>Example</th></tr></thead><tbody><tr><td><br>Postpaid burstable 95th volume Pricing<br></td><td><br>95th percentile bandwidth usage of one instance<br></td><td><br>The price of all the bandwidth units you have used is within the set price range.<br></td><td><br>Assume your actual usage of 95th bandwidth in the billing cycle is 2 Mbps, falling in the 1 Mbps - Unlimited range.<br>Your billing:<br>2 Mbps × 0.50/Mbps = 1.00 zenPoint.<br></td></tr><tr><td><br>Postpaid burstable 95th tiered Pricing<br></td><td><br>95th percentile bandwidth usage of one instance<br></td><td><br>The price per bandwidth unit you have used is within a particular price range. Once you fill up one tier you move to the next.<br></td><td><br>Assume your actual usage of 95th bandwidth in the billing cycle is 2 Mbps, <br>Your billing:<br>0.04 Mbps × 8.00/Mbps + 0.04 Mbps × 4/Mbps + 0.04 Mbps × 2/Mbps + 0.88 Mbps × 1 /Mbps + 1 Mbps × 0.5/Mbps =</td></tr><tr><td><br>Postpaid burstable 95th with commitment<br></td><td><br>95th percentile bandwidth usage of one instance<br></td><td><p><br>You prepay the bandwidth commitment and usage exceeded the base commit rate will be post paid by Mbps.</p><p><img src="../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;"><strong>Note</strong></mark></p><p><mark style="color:blue;">The minimum commitment for each instance is 200 Mbps.</mark><br><mark style="color:blue;"></mark></p></td><td></td></tr></tbody></table>



## Data Transfer

You prepay the bill by month before you use. You are billed by the data transfer.

The data transfer in the data package is only valid within the month (30 days), and data consumed beyond the package will be postpaid by hour.

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">You are highly recommended to buy a sufficient data transfer package according to your actual business.</mark>
{% endhint %}



## Elastic IP

Elastic IP includes ordinary elastic IPs and DDoS protected elastic IPs.

| Elastic IP Type                          | Billing Item                  | Description                                                                                                                                                                                                                                                                                                            |
| ---------------------------------------- | ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><br>Ordinary elastic IP<br></p>       | <p><br>Number of IPs<br></p>  | <p><br>You prepay the IP by month with the price of $3 each.<br><img src="../../.gitbook/assets/Icon.svg" alt="" data-size="line"><mark style="color:blue;"><strong>Note</strong></mark><br><mark style="color:blue;">You can purchase up to 4 EIPs for each instance.</mark><br><mark style="color:blue;"></mark></p> |
| <p><br>DDoS protected elastic IP<br></p> | <p><br>Number of IPs<br> </p> | <p><br>You prepay the IP by month with the price of $99 each.<br></p>                                                                                                                                                                                                                                                  |



## CIDR Block

IPv4 CIDR block and IPv6 CIDR block are supported on zenConsole.&#x20;

| CIDR Block Type                | Billing Item                           | Description                                                                                                                                    |
| ------------------------------ | -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><br>IPv4 CIDR block<br></p> | <p><br>Number of available IPs<br></p> | <p><br>64 available IPs are supported in one zone by default. Please contact us if your required quantity exceeds the  existing stock.<br></p> |
| <p><br>IPv6 CIDR block<br></p> | <p><br>Free for use<br></p>            | <p><br>An IPv6 CIDR block contains 500 available IPs and you can create at most 5 IPv6 CIDR blocks in one zone.<br></p>                        |

