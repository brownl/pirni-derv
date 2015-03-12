**I (brownl) did not write this. I just posted it on GitHub as Google Code is closing.**

What follows is the project summary of pirni-derv, copied from [Google Code](https://code.google.com/p/pirni-derv/). The wiki has also been imported (look in the `wiki` branch).

## Update
The author of Pirni has released a GUI-version of Pirni, entitled "Pirni Pro".

A link to the product is available here: http://moreinfo.thebigboss.org/moreinfo/depiction.php?file=pirniproData

Much of the functionality of 'pirni-derv' is available in Pirni Pro, and is easier to use (No command-line!). However, Pirni Pro is not free ($1.99 via Cydia). I will leave this project open in case people want a free, command-line alternative. 

## derv
![Screenshot](http://i.imgur.com/9DwZJ.png)
### Overview
derv is a collection of scripts for parsing captured network packets; specifically cookies, plain-text passwords, and URLs. derv uses Pirni to capture packets.

Pirni (https://code.google.com/p/n1mda-dev/wiki/PirniUsageGuide) is a packet sniffing application used on iPhone and iPod Touch devices. Pirni is only available for iPhones and iPod Touches which have been [jailbroken](http://www.iphonedownloadblog.com/2009/10/11/jailbreak-iphone-blackra1n-tutorial/). Pirni is available through Cydia and Rock, and requires MobileTerminal to be executed.

Pirni and the derv scripts have been tested on iPhone 3GS and iPod Touch (2nd generation) running OS version 3.0, 3.1, and 3.1.2; should work for all versions of iPhone and iPod OSes that can install and run Mobile Terminal.

### About
Pirni dumps sniffed packets to a file. These packets can be later transferred to a computer and viewed using a packet-viewing program such as [WireShark](http://www.wireshark.org/). This method, however, takes a lot of time and is very byzantine.

I could not find a way to view packets "in realtime" on the iPhone/iPod device as they were being captured, so I wrote these scripts in Bash.

### Scripts
*derv* has two main scripts:

* b4.sh Initiates Pirni with router's IP address, packet filter, port, and filename.
* derv.sh Reads Pirni's packet dump file in 'real time' and displays information gathered from the packets. 

*The other scripts (derv-pw.sh, derv-cookie.sh, derv-url.sh) are required by derv.sh: they should not be run independently or altered.*

### Usage
The purpose of these scripts is to capture and parse packets for passwords, URLs, or cookies. The derv scripts and Pirni are not to be used for illegal or immoral behavior. These tools are meant for auditing network security only.

#### A detailed tutorial on how to install and use derv, Pirni, and Mobile Terminal is now available [here](https://github.com/brownl/pirni-derv/blob/wiki/Installation.md).
