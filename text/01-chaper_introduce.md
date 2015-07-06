# Introduction #

[RT-Thread](http://www.rt-thread.org) is an open source Real-Time operating system for embedded devices from China(you can redistribute it and/or modify it under the terms of GPLv2).It contains lots of components like:Real-time kernel,TCP/IP protocol stack,filesystem,libc interface,graphical user interface and so on.

This manual describes how to use RT-Thread.

## Software Structure of RT-Thread ##

![RT-Thread Software Structure](img/System_Arch.png)

RT-Thread is a real-time operating system divided by different layers, it contains:

* transplant layer and driver layer, this layer is closely related to hardware including drivers and CPU transplant.
* hard real-time kernel, this is the central layer of RT-Thread including the object of kernel system, like multi-threading and its scheduling,semaphore,mailbox,message queue,memory management,timer and so on.
* component layer, this is the expand component base on the kernel,like:filesystem,command line shell interface,LwIP TCP/IP protocol stack,graphical user interface.

RT-Thread has its own characteristics in the aspects of its design and will continue to maintain and develop its characteristics.

* compact kernel and rich component.
* clear,simple,low coupling system architecture.
* Object-Oriented,unix-like coding style.

## Develop && Maintain ##

The development team of RT-Thread almost locate in Shanghai(more precisely,Yangtze River Delta region of China),the developer make use of their spare time to develop and maintain RT-Thread,and at the same time,welcome more developer,embedded system lover,and company to contribute your code to RT-Thread. 

RT-Thread set one year as its publishing cycle.Each versions of RT-Thread will set an goal and in the following year, the development of RT-Thread will surround this goal, and every seasons releases one alpha version, the release version includes:

* stable version,in this version, the new feature should not included in.The changes only includes bugs fix.
* alpha version, its developing cycle last for one year,and it may not stable but contains new features.

Each alpha version sets an goal by means of mail,forum. And one or more developers conference is held in Shanghai every year.In this conference, developer will discuss the goal of new version or its general direction.

The developing activity is divided into different parts according to its software architecture,

* kernel,this is the central and basic part of RT-Thread.
* component,divide the component into different part according to their function,and get its goal:Low coupling, high cohesion.
* porting,it contains the chip transplant and drivers.

This three parts all have maintainer who should guarantee its part's correctness.The developing version located in [GitHub](https://github.com/RT-Thread/rt-thread), welcome to create pull & request.The corresponding maintainer will decide whether this pull & request would be merged.Notice that the code you are contributing to RT-Thread should obey the programming specification set by RT-Thread.




