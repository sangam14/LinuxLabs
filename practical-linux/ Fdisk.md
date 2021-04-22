2. Fdisk

# Partitioning with fdisk

This section shows you how to actually partition your hard drive with the fdisk utility. Linux allows only 4 primary partitions. You can have a much larger number of logical partitions by sub-dividing one of the primary partitions. Only one of the primary partitions can be sub-divided.

Examples:
1) Four primary partitions <br>
2) Mixed primary and logical partitions <br>

# fdisk usage

fdisk is started by typing (as root) fdisk device at the command prompt. device might be something like /dev/hda or /dev/sda (see Section 2.1.1). The basic fdisk commands you need are: <br>
p print the partition table <br>
n create a new partition <br>
d delete a partition <br>
q quit without saving changes <br>
w write the new partition table and exit <br>

Changes you make to the partition table do not take effect until you issue
the write (w) command. Here is a sample partition table:

```
Disk /dev/hdb: 64 heads, 63 sectors, 621 cylinders
Units = cylinders of 4032 * 512 bytes
 Device Boot Start End Blocks Id System
/dev/hdb1 * 1 184 370912+ 83 Linux
/dev/hdb2 185 368 370944 83 Linux
/dev/hdb3 369 552 370944 83 Linux
/dev/hdb4 553 621 139104 82 Linux swap

```
The first line shows the geometry of your hard drive. It may not be
physically accurate, but you can accept it as though it were. The hard
drive in this example is made of 32 double-sided platters with one head on
each side (probably not true). Each platter has 621 concentric tracks. A 3-
dimensional track (the same track on all disks) is called a cylinder. Each
track is divided into 63 sectors. Each sector contains 512 bytes of data.
Therefore the block size in the partition table is 64 heads * 63 sectors *
512 bytes er...divided by 1024. (See 4 for discussion on problems with this
calculation.) The start and end values are cylinders.

```
$fdisk /dev/hdxx
n - create a new partition press <-| at first cylinder
define size +100M at Last cylinder
w - write and quit
$sync
$partprobe -s /dev/hdxx
- rereads the partition table and updates the kernel table.
 -s - to show the output.
```



