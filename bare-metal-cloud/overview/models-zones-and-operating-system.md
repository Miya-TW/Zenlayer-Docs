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

| Region        |   Location   |      City      |                       Zone                      |
| ------------- | :----------: | :------------: | :---------------------------------------------: |
| North America |     U.S.A    |   Los Angeles  |     LAX B, LAX C, LAX D, LAX E, LAX G, LAX H    |
|               |     U.S.A    |     Chicago    |                      CHI A                      |
|               |     U.S.A    |     Dallas     |               DFW A, DFW B, DFW C               |
|               |     U.S.A    |     Atlanta    |                      ATL A                      |
|               |     U.S.A    |   Washington   |               IAD A, IAD D, IAD E               |
|               |     U.S.A    |      Miami     |               MIA A, MIA B, MIA C               |
|               |     U.S.A    |    New York    |               NYC A, NYC B, NYC C               |
|               |     U.S.A    |     Seattle    |                      SEA A                      |
|               |     U.S.A    |    San Jose    |                   SJC A, SJC B                  |
| Latin America |    Brazil    |    Sao Paulo   | SAO A, SAO B, SAO D, SAO E, SAO F, SAO G, SAO I |
|               |    Brazil    | Río de Janeiro |                   GIG B, GIG C                  |
|               |    Brazil    |    Fortaleza   |                      FOR A                      |
|               |    Mexico    |   Mexico City  |                      MEX B                      |
|               |     Chile    |    Santiago    |                      SCL A                      |
|               |   Colombia   |     Bogota     |                      BOG A                      |
| Europe        |    Holland   |    Amsterdam   |               AMS A, AMS C, AMS D               |
|               |    Germany   |    Frankfurt   |        FRA A, FRA B, FRA D, FRA E, FRA F        |
|               |    Turkey    |                |            IST A, IST B, IST C, IST D           |
|               |    England   |     London     |                   LON A, LON B                  |
|               |     Spain    |     Madrid     |                   MAD A, MAD B                  |
|               |    Russia    |     Moscow     |               MOW A, MOW B, MOW C               |
|               |    France    |   Marseilles   |                      MRS A                      |
|               |    France    |      Paris     |               PAR A, PAR B, PAR C               |
|               |     Italy    |      Milan     |                   MXP A, MXP B                  |
|               |    Sweden    |    Stockholm   |                      ARN A                      |
|               |    Poland    |     Warsaw     |                      WAW A                      |
|               |     Asia     |    Thailand    |                   BKK A, BKK D                  |
|               |     India    |    Bangalore   |                   BLR A, BLR B                  |
|               |     India    |     Mumbai     |        BOM A, BOM B, BOM D, BOM E, BOM G        |
|               |     India    |      Delhi     |                   DEL A, DEL C                  |
|               |     India    |     Chennai    |                   MAA A, MAA C                  |
|               |  Bangladesh  |      Dhaka     |                   DAC C, DAC D                  |
|               |      UAE     |      Dubai     |               DXB A, DXB B, DXB C               |
|               |      UAE     |    Fujairah    |                      FJR B                      |
|               |    Israel    |    Tel Aviv    |                      TLV A                      |
|               |     China    |    Hongkong    |            HKG A, HKG B, HKG C, HKG D           |
|               |   Indonesia  |     Jakarta    |            JKT A, JKT D, JKT E, JKT F           |
|               |   Pakistan   |     Karachi    |                      KHI B                      |
|               |   Pakistan   |    Islamabad   |                      ISB B                      |
|               |   Malaysia   |  Kuala Lumpur  |                   KUL A, KUL C                  |
|               |  Philippines |     Manila     |            MNL A, MNL B, MNL E, MNL F           |
|               |  South Korea |      Seoul     |                   SEL A, SEL D                  |
|               |    Vietnam   |   Ho Chi Minh  |                   SGN A, SGN C                  |
|               |    Vietnam   |      Hanoi     |                      HAN B                      |
|               |   Singapore  |    Singapore   |            SIN A, SIN B, SIN C, SIN E           |
|               |    Taiwan    |      Taipe     |               TPE A, TPE C, TPE D               |
|               |     Japan    |      Osaka     |                      OSA A                      |
|               |     Japan    |      Tokyo     |            TYO A, TYO C, TYO D, TYO E           |
| Africa        | South Africa |  Johannesburg  |                   JNB A, JNB B                  |
|               |    Nigeria   |      Lagos     |                   LOS A, LOS B                  |
|               |     Egypt    |      Cairo     |                      CAI A                      |
| Oceania       |   Australia  |     Sydney     |                      SYD A                      |



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

