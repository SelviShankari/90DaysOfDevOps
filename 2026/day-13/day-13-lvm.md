Steps to attach additional volume to any server 

1.) create the volume from the aws console
2.) See if it's status is available
3.) then run "lsblk" command in the server 
With the help of this command you wil get to see list of blocks meaning the list of disks and from there you will also get to see the name of the unmounted volume.


Understanding Disk, Physical Volume, Logical Volume.

1.) Disk:-This is the storage hardware device from which physical volumes will be created .

2.)Physical volume :- It is a part of disk which can be used for making volume groups. Volume groups cannot be directly created from disk.

3.) LVM :- Linux volume manager , sometimes also known as logical volume manager is a storage management system in linux that allows you to manage disks flexibly instead of using fixed partitions.

It allows you to combine multiple disks into one storage pool , Resize stroage anytime, Extend disk wihtout reboot, Create Flexible virtual partitions, Take snapshots for backup.