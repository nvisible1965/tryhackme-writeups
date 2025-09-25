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
