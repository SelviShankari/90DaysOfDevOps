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

-----This is how we give multi-line comment in shell scripting
#!/bin/bash
#This script can input multiple users
#
<<comment
This is a script that cn create multiple inputs and create multiple users so use wisely
comment

---Understanding for loop in shell scripting

*****CODE STARTS HERE*****
#!/bin/bash
#This script can input multiple users
#
<<comment
This is a script that can take multiple inouts and create multiple user so use the command wisely
comment

for i in {1..5}
do
        read -p "Enter the username" user_name

        sudo useradd -m $user_name
        echo "User $user_name added successfully"
done
*****CODE ENDS HERE*****


----- Printing reverse numbers usig shell scripting

*****CODE STARTS HERE*****
for (( num=10 ; num >1 ; num--))
do
        echo $num
done
*****CODE ENDS HERE*****

------Printing the files present in the current directory
*****CODE STARTS HERE*****
for file in ./*
do
        echo $file
done
*****CODE ENDS HERE*****




