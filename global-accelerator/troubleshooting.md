# Troubleshooting

After successfully creating accelerator and setting up DNS record (see [Quick Start](get-started/)), if end users fail to access your website/application, you can follow the next steps to locate the issue:

#### &#x20;**Step 1: Verify the origin server by direct access**

* Access the website/application directly by the origin domain name or IP address through browser to check if the origin server can be accessed normally
* If the access fails in the last step, then telnet the origin IP/domain name & port to check if the port is accessible.&#x20;

Troubleshoot the origin server if the direct access and telnet fail. If the direct access to the origin succeeds, then proceed to the Step 2.

#### &#x20;**Step 2: Verify the connect between user and ZGA PoP**

* Ping the CNAME to check if the request can be forwarded to the IP of ZGA PoP and the latency

&#x20;      _\*Please conduct the action in the same acceleration region where the issue occurs_\
&#x20;      _\*You can find the IP of ZGA PoP  (i.e. VIP) at the accelerator's detail page on  Console_\
&#x20;       __       &#x20;

* If the ping fails, traceroute the domain name (accessed by end user) to locate the exact hop where the issue is

Feedback your testing result in a ticket to Zenlayer Support and we will handle it as soon as possible.\
&#x20;

#### **How to raise a support ticket on Console?**

Click _**Ask Us**_ at the bottom right on Console --> Issue Reporting: complete the information and submit the request.&#x20;

For more self-troubleshooting tips, please go to

[FAQ](faq.md).
