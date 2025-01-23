# Communication protocol

Protocols are required for computers to properly communicate across the network. These include message format, message size, timing, encoding, encapsulation, and message patterns.

- **Message format** - When a message is sent, it must use a specific format or structure.
- **Message size** - The rules that govern the size of the pieces communicated across the network are very strict. They can also be different, depending on the channel used.
- **Timing** - Timing determines the speed at which the bits are transmitted across the network. It also affects when an individual host can send data and the total amount of data that can be sent in any one transmission.
- **Encoding** - Messages sent across the network are first converted into bits by the sending host. Each bit is encoded into a pattern of sounds, light waves, or electrical impulses depending on the network media over which the bits are transmitted.
- **Encapsulation** - Each message transmitted on a network must include a header that contains addressing information that identifies the source and destination hosts. Encapsulation is the process of adding this information to the pieces of data that make up the message.
- **Message pattern** - Some messages require an acknowledgment before the next message can be sent. This type of request/response pattern is a common aspect of many networking protocols. However, there are other types of messages that may be simply streamed across the network, without concern as to whether they reach their destination.

# Communication standards

Topologies allow us to see the networking using representation of end devices and intermediary devices. How does a device see a network? Think of a device in a bubble. The only thing a device sees is its own addressing information. How does the device know it is on the same network as another device? The answer is network protocols. Most network communications are broken up into smaller data units, or packets.

A standard is a set of rules that determines how something must be done. Networking and internet standards ensure that all devices connecting to the network implement the same set of rules or protocols in the same manner. Using standards, it is possible for different types of devices to send information to each other over the internet.

An internet standard is the end result of a comprehensive cycle of discussion, problem solving, and testing. These different standards are developed, published, and maintained by a variety of organizations. When a new standard is proposed, each stage of the development and approval process is recorded in a numbered RFC document so that the evolution of the standard is tracked. RFCs for internet standards are published and managed by the IETF.

# Network communication models

Protocols are the rules that govern communications. Successful communication between hosts requires interaction between a number of protocols. Protocols include HTTP, TCP, IP, and Ethernet. These protocols are implemented in software and hardware that are installed on each host and networking device.

The interaction between the different protocols on a device can be illustrated as a protocol stack. A stack illustrates the protocols as a layered hierarchy, with each higher-level protocol depending on the services of the protocols shown in the lower levels. The separation of functions enables each layer in the stack to operate independently of others.

The suite of TCP/IP protocols that are used for internet communications follows the structure of this model:

- **Application** - Represents data to the user, plus encoding and dialog control
- **Transport** -Supports communication between various devices across diverse networks
- **Internet** - Determines the best path through the network
- **Network Access** - The hardware devices and media that make up the network.

A reference model describes the functions that must be completed at a particular layer but does not specify exactly how a function should be accomplished. The primary purpose of a reference model is to aid in clearer understanding of the functions and processes necessary for network communications.

The most widely known internetwork reference model was created by the OSI project at the International ISO. It is used for data network design, operation specifications, and troubleshooting. This model is commonly referred to as the OSI model.

# OSI model

- **7 – Application** - The application layer contains protocols used for process-to-process communications.
- **6 – Presentation** - The presentation layer provides for common representation of the data transferred between application layer services.
- **5 – Session** - The session layer provides services to the presentation layer to organize its dialogue and to manage data exchange.
- **4 – Transport** - The transport layer defines services to segment, transfer, and reassemble the data for individual communications between the end devices.
- **3 – Network** - The network layer provides services to exchange the individual pieces of data over the network between identified end devices.
- **2 - Data Link** - The data link layer protocols describe methods for exchanging data frames between devices over a common media
- **1 – Physical** - The physical layer protocols describe the mechanical, electrical, functional, and procedural means to activate, maintain, and de-activate physical connections for a bit transmission to and from a network device.
 ![](https://i.imgur.com/ezbN2Z7.gif)
# TCP/IP protocol suite

- **1 - Application Layer**: This is the top layer where user interactions happen. It includes protocols like HTTP (web browsing), FTP (file transfer), and SMTP (email). It handles things like data formatting, encryption, and application-specific communication.
- **2 - Transport Layer**: This layer manages end-to-end communication between devices. The most common protocols here are TCP (Transmission Control Protocol) and UDP (User Datagram Protocol). TCP ensures reliable, ordered delivery of data, while UDP is faster but doesn't guarantee delivery.
- **3 - Internet Layer**: This layer is responsible for routing data between different networks. The key protocol is IP (Internet Protocol), which assigns addresses to devices and handles the forwarding of packets. Other protocols in this layer include ICMP (for error messages) and ARP (for resolving addresses).
- **4 - Link Layer**: This layer is responsible for the physical transmission of data on the network. It handles how data is transmitted over a particular medium (like Ethernet or Wi-Fi) and includes protocols for hardware addressing (e.g., MAC addresses) and error detection.
![](https://i.imgur.com/qkfTLb1.png)
