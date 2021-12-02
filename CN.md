# MODULE 1

## [Introduction](https://www.youtube.com/watch?v=4D55Cmj2t-A&list=PLxCzCOWd7aiGFBD2-2joCpWOLUrDLvVV_&index=2)

![Screenshot from 2021-12-02 19-07-56](https://user-images.githubusercontent.com/42698268/144433306-5f62b9b3-0989-487d-81fb-d64c6208142a.png)

## [Topologies](https://www.youtube.com/watch?v=uDulBxDb7GM&list=PLxCzCOWd7aiGFBD2-2joCpWOLUrDLvVV_&index=5)

![Screenshot from 2021-12-02 19-46-09](https://user-images.githubusercontent.com/42698268/144439190-a96c8532-d16b-4f7a-bd01-68ea6ce6adfd.png)



# OSI Model

![Screenshot from 2021-11-27 00-02-31](https://user-images.githubusercontent.com/42698268/143620144-e4ddcc13-7ef7-4f96-a1b0-7ea368ba34eb.png)


![Screenshot from 2021-11-27 01-44-27](https://user-images.githubusercontent.com/42698268/143626507-97c7199e-a414-40d1-9f88-5e4bf64ffba2.png)

![Screenshot from 2021-11-27 01-53-03](https://user-images.githubusercontent.com/42698268/143626985-78c19731-4802-47a6-9af3-84fe3ce31dbd.png)

![Screenshot from 2021-11-27 01-55-19](https://user-images.githubusercontent.com/42698268/143627091-c83008be-1d53-455a-a1c0-b8359fc90365.png)

 
 
 
 # Layers of OSI Model
 
 OSI stands for Open Systems Interconnection. It has been developed by ISO – ‘International Organization of Standardization‘, in the year 1984. It is a 7 layer architecture with each layer having specific functionality to perform. All these 7 layers work collaboratively to transmit the data from one person to another across the globe. 
 
![computer-network-osi-model-layers](https://user-images.githubusercontent.com/42698268/143621114-3aa72d0c-bc46-4909-a3ac-378e07f99c47.png)


## 1. Physical Layer (Layer 1) :
The lowest layer of the OSI reference model is the physical layer. It is responsible for the actual physical connection between the devices. The physical layer contains information in the form of bits. It is responsible for transmitting individual bits from one node to the next. When receiving data, this layer will get the signal received and convert it into 0s and 1s and send them to the Data Link layer, which will put the frame back together. 

![computer-network-osi-model-layers-bits](https://user-images.githubusercontent.com/42698268/143621202-193817f4-5e33-4122-a444-ecba20900d27.png)

The functions of the physical layer are :  

  1. Bit synchronization: The physical layer provides the synchronization of the bits by providing a clock. This clock controls both sender and receiver thus providing synchronization at bit level.
  2. Bit rate control: The Physical layer also defines the transmission rate i.e. the number of bits sent per second.
  3. Physical topologies: Physical layer specifies the way in which the different, devices/nodes are arranged in a network i.e. bus, star, or mesh topology.
  4. Transmission mode: Physical layer also defines the way in which the data flows between the two connected devices. The various transmission modes possible are Simplex, half-duplex and full-duplex.
  
* Hub, Repeater, Modem, Cables are Physical Layer devices. 
* Network Layer, Data Link Layer, and Physical Layer are also known as Lower Layers or Hardware Layers. 


## 2. Data Link Layer (DLL) (Layer 2) :
The data link layer is responsible for the node-to-node delivery of the message. The main function of this layer is to make sure data transfer is error-free from one node to another, over the physical layer. When a packet arrives in a network, it is the responsibility of DLL to transmit it to the Host using its MAC address. 
Data Link Layer is divided into two sublayers:  

1. Logical Link Control (LLC)
2. Media Access Control (MAC)

The packet received from the Network layer is further divided into frames depending on the frame size of NIC(Network Interface Card). DLL also encapsulates Sender and Receiver’s MAC address in the header.

The Receiver’s MAC address is obtained by placing an ARP(Address Resolution Protocol) request onto the wire asking “Who has that IP address?” and the destination host will reply with its MAC address. 


 ![computer-network-osi-model-layers-framing](https://user-images.githubusercontent.com/42698268/143621438-6c66445a-77e9-41ce-a80e-3e406f8dc4ec.png)

 The functions of the Data Link layer are :  

  1. Framing: Framing is a function of the data link layer. It provides a way for a sender to transmit a set of bits that are meaningful to the receiver. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.
  2. Physical addressing: After creating frames, the Data link layer adds physical addresses (MAC address) of the sender and/or receiver in the header of each frame.
  3. Error control: Data link layer provides the mechanism of error control in which it detects and retransmits damaged or lost frames.
  4. Flow Control: The data rate must be constant on both sides else the data may get corrupted thus, flow control coordinates the amount of data that can be sent before receiving acknowledgement.
  5. Access control: When a single communication channel is shared by multiple devices, the MAC sub-layer of the data link layer helps to determine which device has control over the channel at a given time.

* Packet in Data Link layer is referred to as Frame. 
* Data Link layer is handled by the NIC (Network Interface Card) and device drivers of host machines. 
* Switch & Bridge are Data Link Layer devices. 

## 3. Network Layer (Layer 3) :
The network layer works for the transmission of data from one host to the other located in different networks. It also takes care of packet routing i.e. selection of the shortest path to transmit the packet, from the number of routes available. The sender & receiver’s IP addresses are placed in the header by the network layer. 
The functions of the Network layer are :  

  1. Routing: The network layer protocols determine which route is suitable from source to destination. This function of the network layer is known as routing.
  2. Logical Addressing: In order to identify each device on internetwork uniquely, the network layer defines an addressing scheme. The sender & receiver’s IP addresses are placed in the header by the network layer. Such an address distinguishes each device uniquely and universally.
* Segment in Network layer is referred to as Packet. 
* Network layer is implemented by networking devices such as routers.  

![computer-network-osi-model-layers-packet](https://user-images.githubusercontent.com/42698268/143621597-80fc033f-c7a2-408b-8c6c-939068cb6aac.png)


## 4. Transport Layer (Layer 4) :
The transport layer provides services to the application layer and takes services from the network layer. The data in the transport layer is referred to as Segments. It is responsible for the End to End Delivery of the complete message. The transport layer also provides the acknowledgement of the successful data transmission and re-transmits the data if an error is found. 

* At sender’s side: 
Transport layer receives the formatted data from the upper layers, performs Segmentation, and also implements Flow & Error control to ensure proper data transmission. It also adds Source and Destination port numbers in its header and forwards the segmented data to the Network Layer. 
Note: The sender needs to know the port number associated with the receiver’s application. 
Generally, this destination port number is configured, either by default or manually. For example, when a web application makes a request to a web server, it typically uses port number 80, because this is the default port assigned to web applications. Many applications have default ports assigned. 

* At receiver’s side: 
Transport Layer reads the port number from its header and forwards the Data which it has received to the respective application. It also performs sequencing and reassembling of the segmented data. 

The functions of the transport layer are :  

1. **Segmentation and Reassembly**: This layer accepts the message from the (session) layer, breaks the message into smaller units. Each of the segments produced has a header associated with it. The transport layer at the destination station reassembles the message.
2. **Service Point Addressing**: In order to deliver the message to the correct process, the transport layer header includes a type of address called service point address or port address. Thus by specifying this address, the transport layer makes sure that the message is delivered to the correct process.


The services provided by the transport layer :  

1. **Connection-Oriented Service**: It is a three-phase process that includes 
– Connection Establishment 
– Data Transfer 
– Termination / disconnection 
In this type of transmission, the receiving device sends an acknowledgement, back to the source after a packet or group of packets is received. This type of transmission is reliable and secure.

2. **Connectionless service**: It is a one-phase process and includes Data Transfer. In this type of transmission, the receiver does not acknowledge receipt of a packet. This approach allows for much faster communication between devices. Connection-oriented service is more reliable than connectionless Service.

* Data in the Transport Layer is called as Segments. 
* Transport layer is operated by the Operating System. It is a part of the OS and communicates with the Application Layer by making system calls. 

Transport Layer is called as Heart of OSI model. 


## 5. Session Layer (Layer 5) :
This layer is responsible for the establishment of connection, maintenance of sessions, authentication, and also ensures security. 
The functions of the session layer are :  

  1. **Session establishment, maintenance, and termination**: The layer allows the two processes to establish, use and terminate a connection.
  2. **Synchronization**: This layer allows a process to add checkpoints which are considered synchronization points into the data. These synchronization points help to identify the error so that the data is re-synchronized properly, and ends of the messages are not cut prematurely and data loss is avoided.
  3. **Dialog Controller**: The session layer allows two systems to start communication with each other in half-duplex or full-duplex.
  
* All the below 3 layers(including Session Layer) are integrated as a single layer in the TCP/IP model as “Application Layer”. 
* Implementation of these 3 layers is done by the network application itself. These are also known as Upper Layers or Software Layers. 

SCENARIO: 
Let’s consider a scenario where a user wants to send a message through some Messenger application running in his browser. The “Messenger” here acts as the application layer which provides the user with an interface to create the data. This message or so-called Data is compressed, encrypted (if any secure data), and converted into bits (0’s and 1’s) so that it can be transmitted. 


![computer-network-osi-model-layers-session](https://user-images.githubusercontent.com/42698268/143621845-5c9255c4-df94-48a7-b331-5dac239ee349.png)


## 6. Presentation Layer (Layer 6) :
The presentation layer is also called the Translation layer. The data from the application layer is extracted here and manipulated as per the required format to transmit over the network. 
The functions of the presentation layer are : 

  1. Translation: For example, ASCII to EBCDIC.
  2. Encryption/ Decryption: Data encryption translates the data into another form or code. The encrypted data is known as the ciphertext and the decrypted data is known as plain text. A key value is used for encrypting as well as decrypting data.
  3. Compression: Reduces the number of bits that need to be transmitted on the network.


## 7. Application Layer (Layer 7) :
At the very top of the OSI Reference Model stack of layers, we find the Application layer which is implemented by the network applications. These applications produce the data, which has to be transferred over the network. This layer also serves as a window for the application services to access the network and for displaying the received information to the user. 
Ex: Application – Browsers, Skype Messenger, etc. 

*Application Layer is also called Desktop Layer. 

![computer-network-osi-model-layers-application](https://user-images.githubusercontent.com/42698268/143621949-52506d49-3678-4ea0-8a85-b6f2b0c63360.png)

The functions of the Application layer are :  

  1. Network Virtual Terminal
  2. FTAM-File transfer access and management
  3. Mail Services
  4. Directory Services
  
OSI model acts as a reference model and is not implemented on the Internet because of its late invention. The current model being used is the TCP/IP model. 

# IP addresses

![Screenshot from 2021-11-27 20-40-08](https://user-images.githubusercontent.com/42698268/143686851-229d4b54-32c2-4967-b32b-3ac9ff609a17.png)

* Given is the number of IP addresses you will get if you buy one network either of the class A, or class B, or class C
* But if you have these many IP addresses that doesn't mean that you are going to configure these many hosts
* i.e we can see that you will always be able to use 2 less than the total number of IP addresses, as explained in class A, you can only configure 2^24-1 hosts, and this is true in all classes
  * class A = 2^24 HID || (2^24 - 2) hosts can be configured      || 2^7 networks(NID)
  * class B = 2^16 HID || (2^16 - 2) hosts can be configured(HID) || 2^14 networks(NID)
  * class C = 2^8 HID  || (2^8 - 2) hosts can be configured(HID)  || 2^21 networks(NID)
  * In class D and E, only IP addresses are there, it isn't divided into NID and HID
       * Class D - 2^28 IP addresses - 256 Million addresses are there, but only <1000 are used, so this is its disadvantage 
       * Class E - 2^28 IP addresses( we don't know anyhting about class E)
       * one is used for millitary and other is used for scientific and experimental purposes.


# Network devices 

## 1. Repeater – 
A repeater operates at the physical layer. Its job is to regenerate the signal over the same network before the signal becomes too weak or corrupted so as to extend the length to which the signal can be transmitted over the same network. An important point to be noted about repeaters is that they do not amplify the signal. When the signal becomes weak, they copy the signal bit by bit and regenerate it at the original strength. It is a 2 port device. 

## 2. Hub – 
A hub is basically a multiport repeater. A hub connects multiple wires coming from different branches, for example, the connector in star topology which connects different stations. Hubs cannot filter data, so data packets are sent to all connected devices.  In other words, the collision domain of all hosts connected through Hub remains one.  Also, they do not have the intelligence to find out the best path for data packets which leads to inefficiencies and wastage. 


Types of Hub 

* Active Hub:- These are the hubs that have their own power supply and can clean, boost, and relay the signal along with the network. It serves both as a repeater as well as a wiring center. These are used to extend the maximum distance between nodes.
* Passive Hub :- These are the hubs that collect wiring from nodes and power supply from the active hub. These hubs relay signals onto the network without cleaning and boosting them and can’t be used to extend the distance between nodes.
* Intelligent Hub :- It works like active hubs and includes remote management capabilities. They also provide flexible data rates to network devices. It also enables an administrator to monitor the traffic passing through the hub and to configure each port in the hub.

## 3. Bridge – 
A bridge operates at the data link layer. A bridge is a repeater, with add on the functionality of filtering content by reading the MAC addresses of source and destination. It is also used for interconnecting two LANs working on the same protocol. It has a single input and single output port, thus making it a 2 port device.

Types of Bridges 

* Transparent Bridges:- These are the bridge in which the stations are completely unaware of the bridge’s existence i.e. whether or not a bridge is added or deleted from the network, reconfiguration of the stations is unnecessary. These bridges make use of two processes i.e. bridge forwarding and bridge learning.
* Source Routing Bridges:- In these bridges, routing operation is performed by the source station and the frame specifies which route to follow. The host can discover the frame by sending a special frame called the discovery frame, which spreads through the entire network using all possible paths to the destination.

# 4. Switch –
A switch is a multiport bridge with a buffer and a design that can boost its efficiency(a large number of ports imply less traffic) and performance. A switch is a data link layer device. The switch can perform error checking before forwarding data, which makes it very efficient as it does not forward packets that have errors and forward good packets selectively to the correct port only.  In other words, the switch divides the collision domain of hosts, but broadcast domain remains the same. 
  
# 5. Routers –
A router is a device like a switch that routes data packets based on their IP addresses. The router is mainly a Network Layer device. Routers normally connect LANs and WANs together and have a dynamically updating routing table based on which they make decisions on routing the data packets. Router divide broadcast domains of hosts connected through it.

![Network_devices](https://user-images.githubusercontent.com/42698268/143687632-00ac6775-be40-426f-b8c7-c5316836317b.jpg)


# 6. Gateway – 
A gateway, as the name suggests, is a passage to connect two networks together that may work upon different networking models. They basically work as the messenger agents that take data from one system, interpret it, and transfer it to another system. Gateways are also called protocol converters and can operate at any network layer. Gateways are generally more complex than switches or routers. Gateway is also called a protocol converter. 

# 7. Brouter –
It is also known as the bridging router is a device that combines features of both bridge and router. It can work either at the data link layer or a network layer. Working as a router, it is capable of routing packets across networks, and working as the bridge, it is capable of filtering local area network traffic. 

# 8. NIC – 
NIC or network interface card is a network adapter that is used to connect the computer to the network. It is installed in the computer to establish a LAN.  It has a unique id that is written on the chip, and it has a connector to connect the cable to it. The cable acts as an interface between the computer and router or modem. NIC card is a layer 2 device which means that it works on both physical and data link layer of the network model. 

# Transmission modes:

Transmission mode means transferring data between two devices. It is also known as a communication mode. Buses and networks are designed to allow communication to occur between individual devices that are interconnected. There are three types of transmission mode:- 


![transmissionmodes](https://user-images.githubusercontent.com/42698268/143721740-44e339a7-0d6b-4a31-874f-7c7cbf2406fd.png)

These are explained as following below.

## 1. Simplex Mode –
In Simplex mode, the communication is unidirectional, as on a one-way street. Only one of the two devices on a link can transmit, the other can only receive. The simplex mode can use the entire capacity of the channel to send data in one direction. 
Example: Keyboard and traditional monitors. The keyboard can only introduce input, the monitor can only give the output. 

 
![SiMpleduplex](https://user-images.githubusercontent.com/42698268/143721747-9311e11b-e963-4d1b-a8b5-ca3ecec65c27.png)


## 2. Half-Duplex Mode –
In half-duplex mode, each station can both transmit and receive, but not at the same time. When one device is sending, the other can only receive, and vice versa. The half-duplex mode is used in cases where there is no need for communication in both directions at the same time. The entire capacity of the channel can be utilized for each direction. 
Example: Walkie-talkie in which message is sent one at a time and messages are sent in both directions. 
Channel capacity=Bandwidth * Propagation Delay

![halfduplex](https://user-images.githubusercontent.com/42698268/143721756-124cbfec-1483-4e1b-aa30-41ff20c1c551.png)



## 3. Full-Duplex Mode –
In full-duplex mode, both stations can transmit and receive simultaneously. In full_duplex mode, signals going in one direction share the capacity of the link with signals going in another direction, this sharing can occur in two ways: 

Either the link must contain two physically separate transmission paths, one for sending and the other for receiving.
Or the capacity is divided between signals travelling in both directions. 
 
Full-duplex mode is used when communication in both directions is required all the time. The capacity of the channel, however, must be divided between the two directions. 
Example: Telephone Network in which there is communication between two persons by a telephone line, through which both can talk and listen at the same time. 

Channel Capacity=2* Bandwidth*propagation Delay

![fullduplex](https://user-images.githubusercontent.com/42698268/143721768-f17eaac3-3b39-413f-9ab0-20d749247d00.png)

# Types of Network Topology:


The arrangement of a network that comprises nodes and connecting lines via sender and receiver is referred to as network topology. The various network topologies are:

# [Types of network topology](https://www.geeksforgeeks.org/types-of-network-topology/)








