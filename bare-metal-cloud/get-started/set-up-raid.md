# Set up RAID

## RAID Level <a href="#raid-level" id="raid-level"></a>

RAID (Redundant Array of Independent Disks) creates a single usable data disk, where several physical disks are combined into an array for better speed and fault tolerance. Zenlayer supports the most common RAID types: 0, 1, 5, and 10.

| RAID Levels | Number of disks | Fault Tolerance  | Space Efficiency | Read & Write Performance | Reliability |
| ----------- | --------------- | ---------------- | ---------------- | ------------------------ | ----------- |
| RAID 0      | n ≧ 2           | None             | 100%             | Fast                     | Low         |
| RAID 1      | n ≧ 2           | n/2 disk failure | 50%              | Low                      | High        |
| RAID 5      | n ≧ 3           | 1 disk failure   | (n-1)/n          | Medium                   | Medium      |
| RAID 10     | n ≧ 4           | n/2 disk failure | 50%              | Fast                     | High        |

Application scenarios explanation:

* RAID 0 RAID 0 does not include any redundancy (or backups). That means if one of your disks fails, you lose all the data on that disk. It is primarily used in applications that require high performance and are able to tolerate lower reliability, such as storing temporary files or files that you have backed up elsewhere.
* RAID 1 If you have at least two disks, using RAID 1 will duplicate your data and store a copy on each disk. With high reliability, RAID 1 is usually used for important server or data base storage.
* RAID 5: RAID 5 is a balanced solution with decent processing power as well as some storage space set aside for the redundancies. It is best for storing critical data and running applications that need decent speed and efficiency.
* RAID 10: With high security and relatively high performance, combined the advantages of RAID 0 and RAID 1, RAID 10 is an ideal solution except for the cost. It is best for running applications or hosting servers that need to be up 24/7.



## Prerequisites <a href="#prerequisites" id="prerequisites"></a>

* You should have at least 2 drives to set up RAID.
* Instances with models of LCC, LCE and LCG do not support RAID setup.
* RAID Quick Setup is used for disks with the same storage space, Customized Setup for disks with different storage space.
* If you have more than 4 disks, using RAID 10 instead of RAID 1 in RAID Quick Setup, because RAID 1 needs only 2 disks and the other two will be wasted.



## Set up RAID <a href="#set-up-raid" id="set-up-raid"></a>

After selecting your instance specification, check the **Disk** and **RAID** columns.

<figure><img src="../../.gitbook/assets/image (3) (2).png" alt=""><figcaption><p>Instance Configuration</p></figcaption></figure>

With only 1 disk, the RAID setup is unavailable.

With more than 2 disks:

*   If the disks have different storage space, choose **Customized Setup**.

    Select desired disks to set up different levels.
* If the disks have the same storage space, choose **Quick Setup**
  * Disk number = 2, choose RAID 0 or RAID 1
  * Disk number = 3, choose RAID 0 or RAID 5
  * Disk number ≧ 4 and is even, choose RAID 0, RAID 5 or RAID 10

