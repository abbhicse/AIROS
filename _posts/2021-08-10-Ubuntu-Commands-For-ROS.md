---
title:  "Software Installation"
mathjax: true
layout: post
categories: media
---
## List of GNU/Linux commands

### 1. tree: Display hierarchy of all the folders

Install tree command using following command
```
sudo apt install tree
```
Usage
```
tree <folder name>
```
Example

![Tree example](img/tree.PNG)

### 2. touch: Update the timestamp of a file/Create a file

Usage
```
touch <file name>
```
Example

![Touch example](img/touch.PNG)

### 3. gedit: Open a new file in GUI based text editor

Usage
```
gedit <file name>
```
Example

![Gedit example](img/gedit.PNG)

### 4. ls -la: List the file with permission

Usage
```
ls -la
```

The parameter shown in the left is the permission of a file
For example, **-rw-r--r--**

1. **Read**: Denoted by the letter r. This means that the user can read the file or directory.
2. **Write**: Denoted by the letter w. This means that the user can write or modify the file or directory.
3. **Execute**: Denoted by the letter x. This means that the user can execute the file.
There are also three different user permission groups:

```
Owner: That’s me.

Group: Whatever group the file or directory was assigned to.

All Users: This permission group includes the rest of the users.
```

1. Owner has read and write privileges (i.e. rw-)
2. The group has read privileges (i.e. r–)
3. All other users have only read privileges (r–).

Example


![ls example](img/ls.PNG)


![permission explained](img/permissions-explain.png)



### 4. chmod: Change Mode,Changing permission of a file

Usage
```
chmod [reference][operator][mode] <file_name>_
```

Example
```
chmod +x test.txt, will change the permission to executable
```
![chmod example](img/chmod.PNG)

### 5. export and echo: Helps to store and display a variable in a shell

Usage of export
```
export variable_name=value
```

Usage of echo

```
echo $variable_name
echo "Text"
```

Example

```
export ROS_PATH=/opt/ros
echo $ROS_PATH
```

![export example](img/export.PNG)

## Linux Shell Script

Hellow world shell script

**first.sh**: Print hello world

```
#!/bin/bash
# This is a comment!
echo Hello World        # This is a comment, too!
```

**Running shell script**

The 755 permission

![permission example](img/permission.png)


```
chmod 755 first.sh  
or
chmod +x first.sh
./first.sh

Output: Hello World
```

**second.sh**: Read your name and print with a message

```
#!/bin/bash
echo "Enter Your Name"
read name
echo "Welcome $name to Robocademy"
```

**Running shell script**

```
chmod 755 second.sh  
or
chmod +x second.sh

./second.sh

Output: Enter your name
Lentin
Welcome Lentin to Robocademy
```

**third.sh**: Read a value from command line 

```
#!/bin/bash

arg1=$1
echo "Your value is $arg1"
```

**Running shell script**

```
chmod +x third.sh
./third.sh 123

Output: Your value is 123
```

**fourth.sh**: export variables and echoing it

```
#!/bin/bash

export ROS="Robot Operating System"
echo $ROS
```
**Running shell script**

```
chmod +x fourth.sh
./fourth.sh

Output: Robot Operating System"

```

## The .bashrc file

It is a shell script executing when a new terminal session starts. It is present in /home/<user_name>/folder.

**Opening .bashrc file**

```
gedit ~/.bashrc
```

### source command: Execute commands from a file in the current terminal

Usage

```
source file_name
```

Application: Sourcing environment variables in the current terminal

Example: Sourcing bashrc

```
source ~/.bashrc

```
Example: Sourcing fourth.sh

![source example](img/source.PNG)


## The SSH: Secure shell

Secure protocol for to a remote computer. Useful while connecting to Raspberry Pi, and robot PC.

Installing ssh

```
sudo apt update
sudo apt install openssh-server
```

After installing check the status 

```
sudo systemctl status ssh
```
![ssh example](img/ssh_service.PNG)

```
sudo ufw allow ssh #UFW: Uncomplicated Firewall

ssh

```

![ssh_cmd example](img/ssh.PNG)


**Usage**

```
ssh <user>@<host>

```
**Example**
```
ssh pi@192.168.0.17
```


