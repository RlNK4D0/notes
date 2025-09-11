The **OSI model** is a set of rules that define how devices connect to a network and talk to each other

Its composed of 7 layers
![[Pasted image 20250904000458.png]]

### Layer 1 Physical layer
Physical and composes of [[Ethernet]] and other devices in [[Basics of networking]] 
#### Functions:
- **Bit Synchronization:*** The physical layer provides the synchronization of the bits by providing a clock. This clock controls both sender and receiver thus providing synchronization at the bit level.
- **Bit Rate Control:*** The Physical layer also defines the transmission rate i.e. the number of bits sent per second.
- **Physical Topologies:** Physical layer specifies how the different, devices/nodes are arranged in a network i.e. [bus topology](https://www.geeksforgeeks.org/computer-networks/advantages-and-disadvantages-of-bus-topology/), [star topology](https://www.geeksforgeeks.org/computer-networks/advantages-and-disadvantages-of-star-topology/), or [mesh topology](https://www.geeksforgeeks.org/computer-networks/advantage-and-disadvantage-of-mesh-topology/).
- **Transmission Mode:*** Physical layer also defines how the data flows between the two connected devices. The various transmission modes possible are [Simplex, half-duplex and](https://www.geeksforgeeks.org/computer-networks/difference-between-simplex-half-duplex-and-full-duplex-transmission-modes/) full duplex.

#### Protocols:
- [[USB - Protocol]]
- [[SONET / SDH]]
### Layer 2 Data Link Layer (DLL)
The *DLL* layer is responsible for the node-to-node communication.
The main function of this layer is make sure data transfer is free from errors from one node to other, over the physical layer
It transmits the package to the destinatary using their [[MAC-addresses]], this address is obtained by placing an [[ARP - Address Resolution Protocol]] request on the wire asking, and the destinatary or host will answer with their *MAC address* 
**Switches and bridges** are common DLL devices, seen in [[Basics of networking]]

#### Functions:
- **Framing:** Framing is a function of the data link layer. It provides a way for a sender to transmit a set of bits that are meaningful to the receiver. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.
- **Physical Addressing:*** After creating frames, the Data link layer adds physical addresses (MAC ****addresses***) of the sender and/or receiver in the header of each frame.
- ***Error Control:*** The data link layer provides the mechanism of error control in which it detects and re-transmits damaged or lost frames.
- **Flow Control:*** The data rate must be constant on both sides else the data may get corrupted thus, flow control coordinates the amount of data that can be sent before receiving an acknowledgment.
- **Access Control:*** When a single communication channel is shared by multiple devices, the MAC sub-layer of the data link layer helps to determine which device has control over the channel at a given time.

#### Protocols
- [[Ethernet]]
- [[PPPP]]

### Layer 3 Network layer
The *Network Layer* transmits data from one host to another located in **different networks**, it also takes care of package *routing*.
The sender and receiver's [[IPv4]] or [[IPv6]], are placed in the **Header** of the package 
Common devices in this layer are **Routers and Switches** [[Basics of networking]]

#### Functions:
- ***Routing:*** The network layer protocols determine which route is suitable from source to destination. This function of the network layer is known as routing.
- ***Logical Addressing:*** To identify each device inter-network uniquely, the network layer defines an addressing scheme. The sender and receiver’s IP addresses are placed in the header by the network layer. Such an address distinguishes each device uniquely and universally.

#### Protocols: 
- [[IPv4]]
- [[IPv6]]
- [[ICMP]]
- [[IGMP]]
- [[OSPF]]

### Layer 4 Transport layer
The *transport layer* provides services to the **application layer** and *takes* services from the **Network Layer** 
The data in this layer is referred to as **segments**
It is responsible for the end-to-end delivery of the **Complete** message, it has acknowledgement of the successful data transmission and re-transmits the data if any errors emerge
This layer uses [[TCP]], [[UDP]], [[NetBIOS]], [[PPTP]] protocols

***At the senders side***, This layer receives formatted data from the *upper layers*, performs **Segmentation**, and implements *Flow and Error control* to ensure proper data transmission. It also adds Source and Destination [[Ports-numbers]] in the package header and sends the package to the *Network layer*
- Generally, this destination port number is configured, either by default or manually. For example, when a web application requests a web server, it typically uses port number 80, because this is the default port assigned to web applications. Many applications have default ports assigned.

***At the Receiver’s side,*** Transport Layer reads the port number from its header and forwards the Data which it has received to the respective application. It also performs sequencing and reassembling of the segmented data.

#### Functions:
- **Segmentation and Reassembly:** This layer accepts the message from the *session layer* and breaks the message into smaller units. Each of the segments produced has a header associated with it. The transport layer at the destination station reassembles the message.
- **Service Point Addressing:** To deliver the message to the correct process, the transport layer header includes a type of address called service point address or port address. Thus, by specifying this address, the transport layer makes sure that the message is delivered to the correct process.

#### Services: 
- [[Connection-Oriented-Service]]
- [[Connectionless-Service]]

#### Protocols:
- [[TCP]]
- [[UDP]]
- [[SCTP]]

### Layer 5 Session Layer
This layer is responsible for establishing connections, management of connections, termination of sessions between devices 
It also provides authentication and security

#### Functions:
- **Session Establishment, Maintenance, and Termination:** The layer allows the two processes to establish, use, and terminate a connection.
- **Synchronization:** This layer allows a process to add checkpoints that are considered synchronization points in the data. These synchronization points help to identify the error so that the data is re-synchronized properly, and ends of the messages are not cut prematurely, and data loss is avoided.
- **Dialog Controller:** The session layer allows two systems to start communication with each other in half-duplex or full duplex.

#### Protocols:
- [[NetBIOS]]
- [[PPTP]]
- [[RCP]]

### Layer 6 Presentation Layer
Also called the **Translation Layer**. The data from the *application layer* is extracted and manipulated for the requested format to transmit over the network
Formats like **.JPEG, MPEG, GIF** are standards of formats used for encoding data, which is part of the presentation layer role

#### Functions:
- **Translation:** For example, [ASCII to EBCDIC](https://www.geeksforgeeks.org/computer-organization-architecture/difference-between-ascii-and-ebcdic/).
- **Encryption/ Decryption:** Data encryption translates the data into another form or code. The encrypted data is known as the [[Ciphertext]], and the decrypted data is known as plain text. A key value is used for encrypting as well as decrypting data.
- **Compression:** Reduces the number of bits that need to be transmitted on the network.

#### Protocols:
- [[SSL - Secure Sockets Layer]]
- [[MIME]]

### Layer 7 Application Layer
This **Applications** produce the data that will be transferred to the *lower layers*, this also serves as a window for the application services to access the network and for displaying the received information to the user

#### Functions:
- **Network Virtual Terminal (NVT):** It allows a user to log on to a remote host. [[SSH]]
- **File Transfer Access and Management (FTAM):** This application allows a user to access files in a remote host, retrieve files in a remote host, and manage or control files from a remote computer.
- **Mail Services:** Provide email service.
- **Directory Services:** This application provides distributed database sources and access for global information about various objects and services.

#### Protocols:
- [[SMTP]]
- [[FTP]]
- [[DNS - Domain Name System]]
- [[DHCP]]

### Data Flow in the OSI model
From Sender:
![[Pasted image 20250908165405.png]]

To destination 
![[Pasted image 20250908165453.png]]

## It goes from sender's layer 7 to 1 and for the destination it is the inverse from layer 1 to 7
