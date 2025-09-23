# TryHackMe — Intro to LAN

**Date:** 2025-09-23    

---

## 🔎 Room Overview
* It generally explains LAN topologies, Switch, Routers, ARP, DHCP kind off things.

---
# *LAN Topology*


## What is LAN?
 LAN generally stands for **L**ocal **A**rea **N**etwork. It means as it name refers it is network connection of local area(smaller areas like: schools,offices,library) which is often connected to switch/hub kind off devices.It does have different topologies(structure of devices connected in a network). It has mainly 3 topologies:
#### 1.Star Topology
#### 2.Bus Topology
#### 3.Ring Topology

---

## What is Star Topology
  In this topology, basically we have a centralised device(switch or hub) through which the data is being sent or recieved to other devices connected in the network.
  It can be costy, because of the cost of more cables and the device switch but it is also scalable and reliable.There is also one disadvantage that if there is any fault in centralised device
  then the whole network gets down.
  <img width="1440" height="744" alt="what-is-the-star-topology" src="https://github.com/user-attachments/assets/63f66185-aadd-4b16-a81a-33f679a5e051" />

---


## What is Bus Topology
 * In this all devices are connected to a single cable like all the leaf on a single branch (leaf=device and branch=cable)
 * Cost effective as only need cable to establish connection between devices.
 * Bottleneck and slow if all devices send data or request for data at once.
 * Also then difficult to troubleshoot cause can't find out which device causing this.
 * If cable breaks or get weaks then the whole network fails.

 * <img width="590" height="371" alt="bus-topology-template" src="https://github.com/user-attachments/assets/82e5b738-a4f6-469c-996b-1eaf74e4ab40" />

--- 


### What is Ring Topology
 * Same as Bus Topology but in a loop (circular loop).
 * also known as **Token Topology**
 * Device send data across the loop and other devices send this data forward until it reaches the destined devices. The forwarding device only forward if it doesn't have and data to sent otherwise it also shares it's own data first.
 * Cheap as only cable requires but not fault tolerant as cable may be get weak and broken.
 * <img width="588" height="600" alt="ring-topology2" src="https://github.com/user-attachments/assets/0bce6573-bcfc-4b2b-8360-49b56037f388" />


 ---
---

### What is a Switch?
 * Switch is a device that is used in larger networks to connect many devices at once to send and receive data.
 * It have ports through which devices are connected and unlike hub it doesn't flood the network by copying the data to all the ports it just sends the data to the intended receiver.
 * It can be connected to router which increase relaiability as path of transmission increases but also increase transmission time.

 ---

### What is a Router?
 * It connects two different network on same protocol or different protocol and pass data between them with the help of IP Address and also routing.
 * Routing is choosing the best path from all the paths available for transmission.
 * <img width="550" height="367" alt="router4" src="https://github.com/user-attachments/assets/257197fa-4a6d-4d33-9ef9-a8da18003980" />

 ---
 ---
 ---

 # *Subnetting*

  * Splitting of network into more smaller networks within itself.
  * **Subnet Mask** = Splitting up the No. of hosts can be fitted into a network. It is of 4 bytes (32 bits).
  * It uses IP Address in 3 ways:
     * Identify the **Network Address** = It is the address of start of network tells about existence of network.
     * Identify the **Host Address** = It is the address of host or device on subnet.
     * Identify the **Default Gateway** = It is the address of the first device(router) that sends the data forwards.
     * Benefits:Security,Full Control,Efficiency.
 ---

 # *ARP*

 * Address Resolution Protocol
 * It allows device to assosciate it's Mac address with it's IP address.
 * Device can use ARP to find Mac address of device to communicate by broadcasting into network.
 * **Cache**= *ARP cache* It is the information that is stored to identify the other devices on the network. ARP Request device stores the MAC address in this cache.
 * ARP works in two ways:
    * **ARP request** = Request broadcasted by the device in network asking "What is the MAC address that owns this IP address?" to find.
    * **ARP reply** = Reply sent by the device which own that ip address ( it sends it's MAC address ).
    * <img width="823" height="864" alt="image" src="https://github.com/user-attachments/assets/c00ef229-640b-49bd-89db-39b2a6a0036d" />

  
---

# *DHCP*

 * **D**ynamic **H**ost **C**onfiguration **P**rotocol
 * We assign IP address manually and automatically too by requesting it from DHCP server.
 * Process:
    * If we don't give IP address manually then it will find DHCP server in network for IP address **DHCP discover**
    * Then DHCP server offers an IP or ask that do you want 192.1.1.4 IP address **DHCP offer**
    * Then, we gonna say yes we want that IP address **DHCP request**
    * At last, DHCP server sends an acknowledgment that now we can use this IP address.
  
---

# Thank YOU
     
