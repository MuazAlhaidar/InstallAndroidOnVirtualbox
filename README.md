# InstallAndroidOnVirtualbox

## install needed tools
http://www.android-x86.org/ get the ISO
https://www.virtualbox.org/wiki/VirtualBox get virtual box from either the link or through the command line

## Create the VM
Name: Android
Type: Linux
Version: Linux 2.6 / 3.x / 4.x (32-bit)    Choose the 64-bit version if you downloaded the 64-bit version

Memory size:
Reccomended for 32-bit - 2048MB
Reccomended for 64-bit - 4096MB

Hard Disk File Type: VDI
Hard Disk Size Type: Dynamic

Storage: 8GB Recommended More if you need it

## Install Android on VM
+ When it boots up, choose the Android ISO as the start up disk.
+ When Android Live boots up, choose Installation (not live CD)
+ Choose Craete/Modify Partition.
+ Choose No for GPT
+ When you get into cfdisk, choose New
+ Create a Primary Disk that uses the entire virtual space chosen (8GB in this case)
+ Choose Bootable
+ Choose Write to write the partition
+ Type yes and click enter
+ Once it is finished click quit
+ Select the partition you created
+ Select ext4
+ Choose yes to format the partition
+ Choose yes to GRUB boot loader
+ Choose yes to make /system be read-writable
+ Before choosing to reboot or boot android
  + Go to Virtaul Box Manager > 
          right click your Android VM > 
          Settings > 
          Storage > 
          android ISO > 
          remove the iso from the optical drive (icon on the right of Optical Drive attribute, not remove attachment from the list)
+ Choose Reboot or Boot from the menu

## Using Android VM
+ Choose to not turn on wifi (VM will use the PC's connection)
+ Sign in and finish up
