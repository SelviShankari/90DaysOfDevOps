Linux File System Understanding.

1.) /bin :- /bin stores the command that will be used by all the users wide. It can be said to be a simple toolbox. It contains all the basic commands. The files stored in bin are used for basic system operation. Contains command that are used once the Linux has started. It is used for running scripts also.

2.) /boot :-Stores all the files that are needed to start the linux. Contains files that are used to start linux system.

3.) /dev :- Contains device files (not real files – they represent hardware).
Examples :-
/dev/sda : First hard disk
/dev/tty : Terminal
/dev/null : “Black hole” for Runwanted data.

Linux treats everything as a file – even devices

4.) /etc :- Contains system-wide configuration file. It is used to change hostnames, view password, groups.
Examples :
/etc/passwd : User accounts
/etc/hosts : Local hostname-to-IP mapping
/etc/ssh/ssh_config : SSH configuration 

We can think of /etc as the “control center” for system settings

5.) /home
Each user gets a personal folder here. Example :
/home/ubuntu : Your default login folder. 
User can store personal files and settings here, without affecting the system.

6.) /lib and /lib64
Contain shared libraries needed by system programs (like .dll) files in windows).
Examples :
/lib/x86_64-linux-gnu/libc.so.6  --- Standard C library
/lib/modules/ -- Kernel modules

Without these, commands like ls or cp would not even run.

7.) /media 
Used for temporary mounts (like USB drives or CDs)
Example :
/media/usb : When you plug in a pendrive
Usually managed automatic by system.

8.) /mnt
Traditionally used for manually mounting temporary filesystem.
Example : 
Mounting an EBS volume:
sudo mount /dev/xvdf   /mnt/data

Infra engineers often use /mnt for testing or temporary data storage.

9.) /opt
Stands for optional software – used for third party or custom apps. 
Example:
/opt/google/chrome – Chrome installation directory (in installed)

10.)/var :- Stores variable data ideal for data that keeps on changing. Like storing the logs etc etc

Example:
/var/log:- 
The first place to check when something breaks. 
Examples:
/var/log/syslog – General system logs
/var/log/auth.log – SSH login logs
/var/log/ngnix/ -- Web server logs
/var/log/cloud-init.log – Cloud instance initialization.

11.)/proc & /sys : Virtual files that expose system state. Example: /dev/xvda (EBS volume),
/dev/null , /dev/tty

12.) /tmp :- This folder is used ot store temporary data. In most of  the system it is cleaned while rebooting the system.



Hands on 

1.) 




