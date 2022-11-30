---
layout: default
title: Virtual Machines
parent: Developing in a Linux Environment
nav_order: 1
---

# Virtual Machines
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## What is a Virtual Machine?

## Requirements

You will need to download [ubuntu] desktop and [virtualbox] respectively. 

## Steps

Start by launching virtualbox. To launch a new virtual machine, click the add button at the top.

![](../../assets/vm1.png)

Be sure to name your virtual machine, and for the ISO select the ubuntu deskop ISO you downloaded previously. Then, continue with the process. 

![](../../assets/vm2.png)

You will be asked to create a username and password. This will be the administrator account, or the superuser. Additionally, you can tweek how much memory, disk space, and cpu cores the virtual machine can use. Note that if you give to little resources, the virtual machine may fail to initialize. If at any point in the initialization process the virtual machine fails, try allocating more resources.

![](../../assets/vm3.png)

The virtual machine should open in a new window. After the initialization process finishes, you can login with the username and password you created. To access the command line, click the icon in the bottom left and search for "terminal".

![](../../assets/vm4.png)

[here]: https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox#1-overview
[ubuntu]: https://ubuntu.com/download/desktop
[virtualbox]: https://www.virtualbox.org/