# TryHackMe — OSI-Model

**Date:** 2025-09-23    

---

## 🔎 Room Overview
* It explains about OSI Model and it's 7 layers and their working and protocol.

---


## What is OSI Model?
  * **O**pen **S**ystem **I**nterconnection **M**odel.
  * It is a framework that how all the devices gonna sent, recieve and interpret(understand) the data.
  * **Encapsulation** = Adding of additional info to data header is known as encapsulation.
  * <img width="1024" height="722" alt="image" src="https://github.com/user-attachments/assets/89e900d3-8625-4a11-9d54-f4b4a1cbe578" />
---

## Layer 1 - Physical
  * Lowest layer
  * Frames are put on this layer from data link in bianry form and will transmit in form of electrical signals if we use ethernet cables.
---
## Layer 2 - Data link
  * Physical Addressing (MAC address) of source and destination both.
  * Present the data in a format that is suitable for transmission.
  * Recieves packets from network layer with ip address added and add MAC address which is given by the manufacturer. Inside every computer NIC(network interface card) have unique mac adress to identify it.
---
## Layer 3 - Network
  * **Routing** = Choosing the best path for transmission of packet chunks.
  * *How the best path get selected?* There are mainly 2 protocols:
    * **1.OSPF(Open Shortest Path First)**
    * **2.RIP(Routing Information Protocol)**
    * Factors to decide which route is best are:
        * shortest
        * reliable(is any packet lost before on this path)
        * fastest physical connection (fibre or ethernet)  
  * It also do work of reassembly of packets means combining the data chunks/packets to see the full received data and vice-versa.
---
## Layer 4 - Transport
  * When data is sent, it follows one of the two protocols:
    * **TCP** = Transmission Control Protocol
    * **UDP** = User Datagram Protocol
  *  **TCP**
     * It establishes a connection between devices for a period of time till the data is being sent or recieved by the devices.It provides gurantee(error checking) and reliability.
     * **Advantages:**
      * reliability and accuracy of data.
      * capable of synchronization and prevent the network from flooding of data.
     * **Disadvantages**
      * slower than UDP
      * cause bottleneck for other device
      * requires reliable connection between 2 devices, if one chunk of data is not recieved then whole data is a waste.
     * used for the situation where data needed to be complete and accurate like file sharing, emails or internet browsing.
  
            



