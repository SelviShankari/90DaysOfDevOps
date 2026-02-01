--> What is Operating System ??

    An operating system is an interface between hardware and software. There are different types of OS like Windows , Linux , Mac OS.

--> Understanding Linux 
    Linux is an OS (Operating System) which has a heart called as linux kernel. Linux is an opensoirce system developed by linus torwalds in 1991. 90% of the apps are running on linux. 

    Everything in linux is either a file or a folder (directory).


--> Linux architecture 
    Linux architecture is based on ASKH architecture. 
    A - (Application) Application is the software that is being used by the end user. 

    S - (Shell) Interactive way to talk to the kernel.

    K - (Kernel) Computer programm that understands the commands and modify hardware using binary format.Under the hood Linux uses C and C++ only.

    H - (Hardware) Computer , Monitor , Printer, Speaker.

--> Linux Flavours/Distros (Distribution)
    Ubuntu , CentOS , Fedora , RedHat

--> Understanding process in linux

    Everything in linux is a process.

    what happens when you power on in your laptop ??

    BIOS (Basic Input Output System ) gets triggered. This is the Motherboard which loads the hardware. GNU GRUB (Grand Unified Bootloader acts as the first program to run when the computer boots, loading the operating system kernel into memory). Then we see ubuntu Loading......

    In the backend init process/systemd runs as process id 1 (pid)

    systemd :- systemd is the engine
    systemctl :- system controller is like steering wheel.

--> Process States :- 
     There are different process states that at=re used to identify what a process is actually doing currently.
     Different process states are :- 
     Running , Sleeping , Zombie , Idle etc etc. 
     The roles are defined by the actual word meanings.



Commands that gets used on daily basis:

1.) ping :- To check if the website is reachable or not at network level

2.) curl :- Curl command is used to check of the website can send response or not 

3.) sudo -i :- To get all the sudo privileges

4.)apt install <package-name> :- This command is used ot install any package into our linux system

5.) chmod :- This command is used to change the mode and play with the permission for any file or folder.

