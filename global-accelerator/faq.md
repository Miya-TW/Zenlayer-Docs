# FAQ

#### &#x20;**Setup Sector**

\
**Q:**\
The same origin site has different domain names for user access?\
**A:**\
If you have multiple domain names accessed by users to the same origin site, for example, users in different regions access different domain names, you need to create multiple accelerators because each accelerator can only accelerate one domain name.\
Learn how to [create accelerator](broken-reference).\
&#x20;

#### &#x20;**Troubleshooting Sector**

\
**Q:**\
The acceleration is not as optimized as expected?\
**A:**

1. Confirm whether the CNAME record has been added in your DNS:\
   If the users are accessing the service through domain name, please make sure that the CNAME we provided has been added to your DNS. \
   Learn [how to add DNS record](get-started/add-dns-record.md).
2. Confirm the bandwidth of the origin site:\
   If the bandwidth of the origin site is too low, the file will be loaded slowly, even after the acceleration. It is recommended that you try to increase the origin's bandwidth.
3. Confirm whether the service in the origin is normal:\
   Check the IP address of the origin to see if the service is normal.
4. Confirm the origin region you entered when creating the accelerator matches the real location

\
**Q:**\
When accessing HTTP or HTTPS service, the connect is intermittent?\
**A:**\
When accessing HTTP or HTTPS service, if the connect is intermittent, and all TCP ports cannot be accessed during disconnection.\
After confirm that there are no service exceptions in the origin, you can check whether the server's kernel has been optimized:

```
#cat /etc/sysctl.conf: Check if the following two parameters are 1
net.ipv4.tcp_tw_recycle = 1
net.ipv4.tcp_timestamps = 1
If both are 1, you can modify the value of net.ipv4.tcp_tw_recycle to 0, save and exit
#sysctl -p: Modification succeeds
```
