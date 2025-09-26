# TryHackMe — Packets and Frames

**Date:** 2025-09-25    

---

## 🔎 Room Overview
* In this room we learn a lot of things first we learn about what is packets and frames and then something more about TCP/IP(Three way handshake) with practical and then about UDP and at last we know about how the ports work and open.

---


## What is Packets and Frames?
  * Both are just small packets of data which forms together to create a larger piece of information.
  * Packets is piece of data from Layer 3 of OSI Model (Network Layer) contain information such as IP address and data payload.
  * While Frame is a piece of data from Layer 2 of OSI Model (Data Link Layer) adds information such as MAC address and encapsulate the packet(adding more data).
  * Bottlenecks are less because of small data pieces and no larger piece of data sent at once that makes the transmission speed slow.
  * **Example** = If we request a image from a website it will not come full image at once instead the image will sent into different packets of data which our computer recieves and re-assamble to display the whole image.
  * And as we know, In Networking there is rules and protocols for almost everything so the way a packets get handled because there can be different structured packets we need standardisation so the things don't get messy.
  * We use Internet Protocol(IP) for packets, and the packets which are using this protocol will have different header which contains additional piece of information along with data.
      * **Time To Live(TTL)** - It is the expiry timer of packet if the packet doesn't reach or get lost then it will expire and doesn't clog the network.
      * **Checksum** - This provide integrity and error checking the reciever checks value of this if it's not the standard value that means the data get either lost or corrupted.
      * **Source Address** - It is the IP address of device from where data packet is sent to and where the acknowledgement need to send.
      * **Destination Address** - It is the IP address of device which recieves the sent data.

---

## TCP/IP (Three Way Handshake)
 * Transmission Control Protocol.
 * It is similar to OSI Model and created before OSI Model and have only 4 layers which are as follows:
   * **1.Application**
   * **2.Transport**
   * **3.Internet**
   * **4.Network Interface**
 * Connection based protocol it means it establish a connection between the client and the server before the data is sent.
 * **Advantages**
   * Gurantee Integrity(No errors)
   * Provide synchronisation as connection based.
   * Performs lot more processes for reliability.

 
 * **Disadvantages**
   * Slower than UDP because more work has to be done.
   * Can cause bottleneck for other device as connection is based between two devices.  
   * Requires reliable connection as one piece of data is not recieved the whole data become useless and must be resent.
 <br>
 
 * **Encapsulation** = Information is added to each layer of model as header this process is encapsultaion.
 
 
 * Some cruical headers are as follows:
   * **Source Port** - It is the value of port that is opened by the sender to send the TCP Packet. It is a random number between 0-65535.
   * **Destination Port** - It is the port number on which the application or service is running on unlike the source port it is not choosen random it is fixed.(Webserver on Port 80)
   * **Source IP** - It is the IP address of the device which is sending the data
   * **Destination IP** - It is the IP address of the device which is receiving the data.
   * **Sequence Number** - When connection occurs, the first piece of data is given a random number.
   * **Acknowledgement Number** - After the first piece of data the second piece of data is given the sequence number +1 this is the acknowledgment number.
   * **Checksum** - Provides integrity to TCP. It is value of sum which is checked by the reciever if it's value is correct(expected value) then data is correct but if value is not same then the data maybe missing or corrupted.
   * **Data** - This is the main data which is to be transmitted.
   * **Flag** - This header determines how the packets should be handled by the other device.Different flags shows different behaviours and meanings.


   <br>

   ### Three Way Handshake
    * It is the process of how TCP establish connection between the two devices.
    * Special messages or Flags of Three Way Handshake is :
      * **SYN** - A SYN is the initial packet sent by a client to initiate a connection and establish it and synchronise the two devices.
      * **SYN/ACK** - This is the acknowledgment sent by the server(receiving device) acknowledging the attempt of sychronisation from client.
      * 
