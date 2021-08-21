---
title:  "Software Installation"
mathjax: true
layout: post
categories: media
---
### VMware Installation

[Install VMware Workstation Player On Windows 10](https://windows.tutorials24x7.com/blog/how-to-install-vmware-workstation-player-on-windows-10)

### Ubuntu Installation

[Install Ubuntu 20.04 LTS On Windows Using VMware Workstation Player](https://ubuntu.tutorials24x7.com/blog/how-to-install-ubuntu-20-04-lts-on-windows-using-vmware-workstation-player)

### ROS 1 Installation

[Install ROS Noetic on Ubuntu 20.04](https://varhowto.com/install-ros-noetic-ubuntu-20-04/)

### Python Installation Optional

[Install Python 3 on Ubuntu 18.04 or 20.04](https://phoenixnap.com/kb/how-to-install-python-3-ubuntu)

``` sudo apt install idle ```

### Anaconda Installation

- [Follow step 1](https://linuxize.com/post/how-to-install-anaconda-on-ubuntu-20-04/)

- [Download the Latest Version of Anaconda](https://www.anaconda.com/products/individual)

- Go to the download folder using your ubuntu command terminal:

  ``` cd /home/abbhicse/Downloads ```

- [Follow step 4 to step 6](https://phoenixnap.com/kb/how-to-install-anaconda-ubuntu-18-04-or-20-04#ftoc-heading-4)

### JupyterLab and Notebook Installation

[Installing the Jupyter Software](https://jupyter.org/install)

### A Jupyter Kernel For C++ Installation

[xeus-cling](https://github.com/jupyter-xeus/xeus-cling)


### Install THE Unofficial Jupyter Notebook Extensions

It has some interesting extensions (e.g. spell checker, collapsible headings, ...). One of the extensions is [Export HTML With Embedded Images](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/nbextensions/export_embedded/readme.html) which exactly does what you want.

To install [Nbextensions](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/) do the following:

```conda install -c conda-forge jupyter_contrib_nbextensions```

Then you will see in your Jupyter homepage a new tab (Nbextensions), where you can enable and configure different extension.
After enabling the "Export HTML With Embedded Images", you will see the corresponding option in the "File-Download as" menu.

### Jupyter-ROS Insatallation Optional for them who want to use ROS with jupyter
- [ROS Noetic](https://github.com/RoboStack/ros-noetic)
- [Jupyter-ROS](https://github.com/RoboStack/jupyter-ros)
- [JupyterLab-ROS](https://github.com/RoboStack/jupyterlab-ros)

### Running C++ With ROS In Jupyter Using Xeus-Cling

[rapyuta-robotics blog](https://github.com/rapyuta-robotics/jupyter_ros_utils)

### Mounting VMware Shares from the Command Line on Linux VM

- Left click on ubuntu 64 bit virtual disk image file
- Right click on setting 
- Under ```Option``` tab, right click on ```Shared Folders```
- Select the option ```Always enabled``` and then click on ```Add```
- Then click ```Next``` and browse to the already created shared folder in windows 10 desktop
- Now click ```Next``` and then ```Finish``` and then ok
- Next power on the ubuntu image file
- Now go to ```etc``` folder under root directory by the command: ``` cd /etc```
- Now edit fstab file via this command: ```gedit fstab``` and add: ```vmhgfs-fuse    /mnt/hgfs    fuse    defaults,allow_other    0    0 ```
- Make sure the target folder exists. If not: ```sudo mkdir /mnt/hgfs```
- Then remount: ```sudo mount -a```

### Some Problems

Problem 1: ``` /usr/bin/env: ‘python’: No such file or directory ```

Solution 1: ``` sudo apt-get install python3 ```

Solution 2: ``` whereis python3 ``` and then: ```sudo ln -s /usr/bin/python3 /usr/bin/python  ```
