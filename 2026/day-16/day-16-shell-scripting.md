-- What is a Shell ?
A shell is a programm that acts as an interface between the user and the Linux operating system (kernal)

There are different varieties of shell based on the operating system you use

1.) bydefault shell is called as sh (shell)
2.) the one which comes is linux is called as bash (bourne shell)
3.) in mac os it is called as zsh
4.) there is another variant also called as csh (corn shell)

--Taking user inputs in shell scripting (for syntax refer to the below code snippet)


*****CODE STARTS HERE*****
#!/bin/bash
# This is the script for variable practice
#
read -p "Enter you name:" Name
echo $Name
*****CODE ENDS HERE*****

read -p : This takes input from the user
echo : anything written after echo gets printed.

-- Refer to the below code which updates the server and installs the package

*****CODE STARTS HERE*****
#!/bin/bash
#
echo "Wait until the server is getting updated"
sudo apt update
echo "The Server has been successfully updated"
read -p "Now enter the package name you want to install" package
sudo apt install $package -y
echo "The package also have been installed successfully "
*****CODE ENDS HERE*****


-- Checking greater than and lesser than 

*****CODE STARTS HERE*****
#!/bin/bash
a=20
b=10

if [ $a -gt $b ] ; then
        echo "$a is greater than $b"
else
        echo "$b is greater then $a"
fi
*****CODE ENDS HERE*****





