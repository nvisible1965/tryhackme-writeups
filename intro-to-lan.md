# TryHackMe — Intro to LAN

**Date:** 2025-09-23    

---

## 🔎 Room Overview
* It generally explains LAN topologies, Switch, Routers, ARP, DHCP kind off things.

---

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

 
