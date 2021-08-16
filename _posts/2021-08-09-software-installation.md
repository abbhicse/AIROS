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

### Python Installation

[Install Python 3 on Ubuntu 18.04 or 20.04](https://phoenixnap.com/kb/how-to-install-python-3-ubuntu)

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

To install [Nbextensions](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/) using pip do the following:

```
   pip install jupyter_contrib_nbextensions
   pip install jupyter_nbextensions_configurator
   jupyter contrib nbextension install --user 
   jupyter nbextensions_configurator enable --user
   
```
Then you will see in your Jupyter homepage a new tab (Nbextensions), where you can enable and configure different extension.
After enabling the "Export HTML With Embedded Images", you will see the corresponding option in the "File-Download as" menu.

### Jupyter-ROS Insatallation : Optional[Who want to use ROS with jupyter]
- [ROS Noetic](https://github.com/RoboStack/ros-noetic)
- [Jupyter-ROS](https://github.com/RoboStack/jupyter-ros)
- [JupyterLab-ROS](https://github.com/RoboStack/jupyterlab-ros)
