# Models, Zones & Operating System

## **Models**

Zenlayer bare metal instance has three main models with different configurations. The table below displays the main parameters as reference.

| S                                                                                                                                                   | M                                                                                                                                                                                     | L                                                                                                                                                                                      |
| --------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>Processor: Single E3</li><li>RAM: 16GB or more</li><li>NIC: 2*10Gbps</li><li>Storage: SATA</li><li>IPMI Access</li><li>Dual Power</li></ul> | <ul><li>Processor: Dual E5 or higher</li><li>RAM: 64GB or more</li><li>NIC: 4*10Gbps</li><li>Storage: SAS/SATA</li><li>Hardware RAID</li><li>IPMI Access</li><li>Dual Power</li></ul> | <ul><li>Processor: Dual E5 or higher</li><li>RAM: 128GB or more</li><li>NIC: 4*10Gbps</li><li>Storage: SAS/SATA</li><li>Hardware RAID</li><li>IPMI Access</li><li>Dual Power</li></ul> |

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

<mark style="color:blue;">The specific configuration may change, which is subject to the data on the opening page of zenConsole.</mark>
{% endhint %}

****

## **Zones**

Bare metal instances are deployed by zones. Each zone has its own power grid and network structure. Your instances in the same zone can buildup private network by Virtual Private Cloud and clusters with Internet access by Public Virtual Interface.

The table below displays the cities and zones that are available, but the accurate data is subject to the opening page on zenConsole.

| Region                        |              City             |                          Zone                          |
| ----------------------------- | :---------------------------: | :----------------------------------------------------: |
| Americas                      |          Los Angeles          |               LAX C, LAX H, LAX I, LAX G               |
|                               | Los Angeles - China Optimized |                   LAX B, LAX D, LAX E                  |
|                               |            Chicago            |                          CHI A                         |
|                               |             Dallas            |                   DFW A, DFW B, DFW C                  |
|                               |            Atlanta            |                          ATL A                         |
|                               |           Washington          |               IAD A, IAD D, IAD E, IAD F               |
|                               |             Miami             |                   MIA A, MIA B, MIA C                  |
|                               |            New York           |                   NYC A, NYC B, NYC C                  |
|                               |            Seattle            |                          SEA A                         |
|                               |            San Jose           |                      SJC A, SJC B                      |
|                               |           Sao Paulo           | SAO A, SAO B, SAO D, SAO E, SAO F, SAO H, SAO I, SAO G |
|                               |         Río de Janeiro        |                      GIG B, GIG C                      |
|                               |           Fortaleza           |                          FOR A                         |
|                               |          Mexico City          |                          MEX B                         |
|                               |           Santiago            |                         SCL A                          |
|                               |             Bogota            |                          BOG A                         |
|                               |          Buenos Aires         |                          EZE A                         |
| Asia Pacific                  |            Bangkok            |                      BKK A, BKK D                      |
|                               |           Bangalore           |                      BLR A, BLR B                      |
|                               |             Yangon            |                          RGN D                         |
|                               |             Medan             |                          KNO A                         |
|                               |             Mumbai            |        BOM A, BOM B, BOM D, BOM E, BOM G, BOM H        |
|                               |             Delhi             |                      DEL A, DEL C                      |
|                               |            Chennai            |                      MAA A, MAA C                      |
|                               |             Dhaka             |                      DAC C, DAC D                      |
|                               |           Hong Kong           |               HKG A, HKG B, HKG D, HKG E               |
|                               |  Hong Kong - China Optimized  |                          HKG C                         |
|                               |            Jakarta            |               JKT A, JKT D, JKT E, JKT F               |
|                               |            Karachi            |                          KHI B                         |
|                               |           Islamabad           |                          ISB B                         |
|                               |          Kuala Lumpur         |                      KUL A, KUL C                      |
|                               |             Manila            |               MNL A, MNL B, MNL E, MNL F               |
|                               |             Seoul             |                      SEL A, SEL D                      |
|                               |          Ho Chi Minh          |                      SGN A, SGN C                      |
|                               |             Hanoi             |                          HAN B                         |
|                               |           Singapore           |               SIN A, SIN B, SIN C, SIN E               |
|                               |             Taipei            |                   TPE A, TPE C, TPE D                  |
|                               |             Osaka             |                          OSA A                         |
|                               |             Tokyo             |                   TYO A, TYO C, TYO E                  |
|                               |    Tokyo - China Optimized    |                          TYO D                         |
|                               |             Sydney            |                          SYD A                         |
| Europe Middle East and Africa |           Amsterdam           |                   AMS A, AMS C, AMS D                  |
|                               |           Frankfurt           |            FRA A, FRA B, FRA D, FRA E, FRA F           |
|                               |            Istanbul           |               IST A, IST B, IST C, IST D               |
|                               |             London            |                      LON A, LON B                      |
|                               |             Madrid            |                      MAD A, MAD B                      |
|                               |             Moscow            |                   MOW A, MOW B, MOW C                  |
|                               |           Marseilles          |                          MRS A                         |
|                               |             Paris             |                   PAR A, PAR B, PAR C                  |
|                               |             Milan             |                      MXP A, MXP B                      |
|                               |           Stockholm           |                          ARN A                         |
|                               |             Warsaw            |                          WAW A                         |
|                               |             Dubai             |                   DXB A, DXB B, DXB C                  |
|                               |            Fujairah           |                          FJR B                         |
|                               |            Tel Aviv           |                          TLV A                         |
|                               |          Johannesburg         |                      JNB A, JNB B                      |
|                               |             Lagos             |                      LOS A, LOS B                      |
|                               |             Cairo             |                          CAI A                         |



## **Operating System**

| Operating System |                                                                                          Version                                                                                          |
| :--------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|      Centos      |                                          <p>CentOS7.4-x86_64<br>CentOS7.5-x86_64<br>CentOS7.6-x86_64<br>CentOS7.8-x86_64<br>CentOS8.0-x86_64</p>                                          |
|      Debian      |                                                           <p>Debian10.6-x86_64<br>Debian8.11.0-x86_64<br>Debian9.8.0-x86_64</p>                                                           |
|      Ubuntu      |                                                           <p>Ubuntu16.04-x86_64<br>Ubuntu18.04-x86_64<br>Ubuntu20.04-x86_64</p>                                                           |
|       ESXI       |                                                                 <p>VMware-ESXi6.0<br>VMware-ESXi6.5<br>VMware-ESXi6.7</p>                                                                 |
|      Windows     | <p>Win2012-R2-DC-CN<br>Win2012-R2-DC-EN<br>Win2012-R2-SE-CN<br>Win2012-R2-SE-EN<br>Win2016-DC-CN<br>Win2016-DC-EN<br>Win2019-DC-CN<br>Win2019-DC-EN<br>Win2019-SE-CN<br>Win2019-SE-EN</p> |

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">More operating systems will be supported.</mark>&#x20;
* <mark style="color:blue;">Some models may not support certain operating systems.</mark>
{% endhint %}

