# Virtual Private Cloud

## What is a virtual private cloud?

A virtual private cloud (VPC) is a virtual network that closely resembles a traditional network that you'd operate in your own data center. Resources in the same VPC can communicate with each other. After you create a VPC, you can add subnets.

### **Supported Zones**

You can create a VPC in the availability region. An availability region consists of several bare metal zones, for example, Atl-A and Atl-B.&#x20;

The table below shows the cities and zones that support VPC, but the accurate data is subject to the opening page on zenConsole.

| Region                           | City                          | Zone                                                   |
| -------------------------------- | ----------------------------- | ------------------------------------------------------ |
| North, Central and South America | Chicago                       | CHI1A                                                  |
| North, Central and South America | Los Angeles                   | LAX2G, LAX2H, LAX2I, LAX5C                             |
| North, Central and South America | Los Angeles - China Optimized | LAX5D, LAX5E                                           |
| North, Central and South America | Miami                         | MIA2A, MIA2B, MIA2C                                    |
| North, Central and South America | New York                      | NYC1A                                                  |
| North, Central and South America | São Paulo                     | SAO2A, SAO2B, SAO2D, SAO2E, SAO3H, SAO4F, SAO4G, SAO4I |
| North, Central and South America | Seattle                       | SEA1A                                                  |
| North, Central and South America | San José                      | SJC2A, SJC2B                                           |
| Asia and Pacific                 | Bangkok                       | BKK1A                                                  |
| Asia and Pacific                 | Mumbai                        | BOM2A, BOM3B, BOM3D, BOM3G, BOM3H, BOM5E               |
| Asia and Pacific                 | Dhaka                         | DAC3D                                                  |
| Asia and Pacific                 | Hanoi                         | HAN1B                                                  |
| Asia and Pacific                 | Hong Kong                     | HKG5A, HKG7B                                           |
| Asia and Pacific                 | Hong Kong - China Optimized   | HKG5C                                                  |
| Asia and Pacific                 | Islamabad                     | ISB2B                                                  |
| Asia and Pacific                 | Jakarta                       | JKT3A, JKT3D, JKT3E,                                   |
| Asia and Pacific                 | Karachi                       | KHI2B                                                  |
| Asia and Pacific                 | Kuala Lumpur                  | KUL2A, KUL2C                                           |
| Asia and Pacific                 | Chennai                       | MAA2A, MAA2C                                           |
| Asia and Pacific                 | Manila                        | MNL2A, MNL3B                                           |
| Asia and Pacific                 | Seoul                         | SEL2A, SEL2D                                           |
| Asia and Pacific                 | Ho Chi Minh City              | SGN3A, SGN4C                                           |
| Asia and Pacific                 | Singapore                     | SIN3A, SIN3B, SIN6C                                    |
| Asia and Pacific                 | Sydney                        | SYD1A                                                  |
| Asia and Pacific                 | Taipei                        | TPE3A, TPE4C, TPE4D                                    |
| Asia and Pacific                 | Tokyo                         | TYO2A, TYO5C                                           |
| Asia and Pacific                 | Tokyo - China Optimized       | TYO5D                                                  |
| Europe, Middle East and Africa   | Amsterdam                     | AMS2C                                                  |
| Europe, Middle East and Africa   | Dubai                         | DXB1A, DXB1B                                           |
| Europe, Middle East and Africa   | Frankfurt                     | FRA5B, FRA5D, FRA5E, FRA9F                             |
| Europe, Middle East and Africa   | Johannesburg                  | JNB1A                                                  |
| Europe, Middle East and Africa   | London                        | LON1A                                                  |
| Europe, Middle East and Africa   | Lagos                         | LOS1A, LOS1B                                           |
| Europe, Middle East and Africa   | Madrid                        | MAD2B                                                  |
| Europe, Middle East and Africa   | Moscow                        | MOW1A, MOW3B, MOW3C                                    |
| Europe, Middle East and Africa   | Milan                         | MXP1A, MXP1B                                           |
| Europe, Middle East and Africa   | Paris                         | PAR2B                                                  |



## **What is a subnet?**

A subnet is a range of IP addresses in your VPC. You can launch your resources into a specific subnet to protect your applications from the failure of a single zone.. When you create a subnet, you specify the IPv4 CIDR block for the subnet, which is a subset of the VPC CIDR block.

