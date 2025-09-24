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
  * **UDP**
    * No error checking,connectionless,doesn't provide gurantee and not reliable as much as TCP and no sychrozation.
      * **Advantages**
       * Faster than TCP
       * Connectionless so no bottleneck
       * It leaves on Application layer to decide how fast the packet should move.
     * **Disdvantages**
       * It doesn't care if data is being recieved or not.
       * Unstable connection due to which user may face terrible issues.
    * Useful for small data to sent.
    * Protocols used for discovering devices, Video calls where pixels can be used, larger files.
 ---
 ## Layer 5 - Session
  * It creates and maintains the connection to the other device.When connection is established, the session is created.
  * It is also responsible for closing of connection if it is not being used or lost.
  * Session also have 'Checkpoints' so when data get lost only the newest data needed to be resent and this saves the bandwidth(capacity of a link to transmit data).
---
## Layer 6 - Presentation
 * Standardisation happens that means if any software developer built email client software but the data still needed to be handled the same way doesn't matter how the software works.
 * Translator as the data sent to other device which is not in understandable format by other device then this layer translate that data and display it as needed.
 * Encryption of data happens and give security to data
---
### Layer 7 - Application
 * Protocols determines how the user should interact with data sent or recieved.
 * Applications like email client software, internet browser, file sharing browser provides Graphical User Interface(GUI) for user to interact.
 * DNS protocol is also on application layer it is how the website addresses in numbers IP 192.168.1.1 is into domain name system like tryhackme.com.
---
---
---
# Thank You
            
