Understanding Disk, Physical Volume, Logical Volume.

1.) Disk:-This is the storage hardware device from which physical volumes will be created .

2.)Physical volume :- It is a part of disk which can be used for making volume groups. Volume groups cannot be directly created from disk.

3.) LVM :- Linux volume manager , sometimes also known as logical volume manager is a storage management system in linux that allows you to manage disks flexibly instead of using fixed partitions.

It allows you to combine multiple disks into one storage pool , Resize stroage anytime, Extend disk wihtout reboot, Create Flexible virtual partitions, Take snapshots for backup.


When to directly mount the volume ??
When the usecase is small and the requirement is clear or predefined with certain amount of storage at that time we can dierctly mount  the volume. 

Steps to mount additional volume directly to any server 

1.) create the volume from the aws console
2.) See if it's status is available
3.) then run "lsblk" command in the server 
With the help of this command you wil get to see list of blocks meaning the list of disks and from there you will also get to see the name of the unmounted volume.
4.) declare the filesystem type using mkfs command.
5.) Mount the volume

Steps to mount the volume and making it flexible, extendable
1.) create the volume from the aws console
2.) See if it's status is available
3.) run lsblk command to see the name of the device
4.) Create physical volume from the storage that is attached
5.) Create a volume group of the physical volume 
6.) Create a logical volume and allocate the required amount of storagr you need from the volume manager
7.) Mount the volume
8.) Start using it.


