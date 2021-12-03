# MODULE 1
![CNmodule1](https://user-images.githubusercontent.com/76476144/144490890-27d68f02-a800-4506-b1f6-9a5e925e4bf7.jpeg)

# 0. Representation of data and its flow network

## Data Representation
* Data refers to the symbols that represent people, events, things, and ideas. Data can be a name, a
number, the colors in a photograph, or the notes in
a musical composition.
* Data Representation refers to the form in which data is stored, processed, and transmitted.
* Devices such as smartphones, iPods, and computers store data in digital formats that can be handled by electronic circuitry
* Digitization is the process of converting information, such as text, numbers, photo, or music, into digital data that can be manipulated by electronic devices.
* The Digital Revolution has evolved through four phases, beginning with big, expensive, standalone computers, and progressing to today’s digital world in which small, inexpensive digital devices are everywhere.
* The 0s and 1s used to represent digital data are referred to as binary digits — from this term we get the word bit that stands for binary digit.
* A bit is a 0 or 1 used in the digital representation of data.
* A digital file, usually referred to simply as a file, is a named collection of data that exits on a storage medium, such as a hard disk, CD, DVD, or flash drive.




# 1.L -2 [Introduction](https://www.youtube.com/watch?v=4D55Cmj2t-A&list=PLxCzCOWd7aiGFBD2-2joCpWOLUrDLvVV_&index=2)
* A computer network is a collection of various computing devices, and it's purpose is to share the data by connecting various heterogenous and homogeneous devices


![Screenshot from 2021-12-03 13-44-54](https://user-images.githubusercontent.com/42698268/144570678-68aa65a1-a1d7-496a-a068-7a553048ce57.png)

* Connection is created while sending data from sender to receiver
* some protocols are defined for both sender and receiver to make communication meaningful

![Screenshot from 2021-12-03 13-45-01](https://user-images.githubusercontent.com/42698268/144570684-0c971cc0-50b5-4819-aad3-dc4a7e0ecf0c.png)

* If sender and rcvr are in same machine then communication is very fast and easy but when sender and rcvr are different machines, and present in different countries, still communication between them is very fast and it does not feel like that we are fetching data from the server present in another country
* And the communication which is happening between them is following some rules and have functionalities


![Screenshot from 2021-12-03 13-49-24](https://user-images.githubusercontent.com/42698268/144570690-110d6540-6ff0-45dc-8342-5ba837a881f9.png)


![Screenshot from 2021-12-03 13-52-29](https://user-images.githubusercontent.com/42698268/144570705-483f4871-a982-4e8d-aeb2-dc58c7548f81.png)
* Error control - To keep check that the data which is getting transferred is not interferred by some external sound, hacker or something else which would change the original data, i.e data should be unchanged and original
* Flow control - Buffer should be fully filled, which would result in congestion
* MUX, DEMUX - If our system is receiving msg or mail, then which particular process would handle it

![Screenshot from 2021-12-03 13-59-41](https://user-images.githubusercontent.com/42698268/144570712-0554853d-c50c-4a0a-8af1-aff3ce5fb517.png)

# L - 3. TCP/IP protocol suite

* Why different - because OSI model is theoretical model and is fundamental and TCP/IP model is implementable model
![Screenshot from 2021-12-03 16-07-29](https://user-images.githubusercontent.com/42698268/144588714-60fb18a2-06ac-4b1c-a7fe-66a80e037a8b.png)

# L- 4 Physical layer in computer networks

![Screenshot from 2021-12-03 16-15-27](https://user-images.githubusercontent.com/42698268/144590023-a6c70e77-3db6-4b01-acd9-081271b735c8.png)

![Screenshot from 2021-12-03 16-15-53](https://user-images.githubusercontent.com/42698268/144590042-627e185e-2672-439e-b24c-b3f1828f0094.png)


# L - 5 Types of Network Topology:


The arrangement of a network that comprises nodes and connecting lines via sender and receiver is referred to as network topology. The various network topologies are:

# [Types of network topology](https://www.geeksforgeeks.org/types-of-network-topology/)


## [Topologies](https://www.youtube.com/watch?v=uDulBxDb7GM&list=PLxCzCOWd7aiGFBD2-2joCpWOLUrDLvVV_&index=5) Mesh and Star

![Screenshot from 2021-12-02 19-46-09](https://user-images.githubusercontent.com/42698268/144439190-a96c8532-d16b-4f7a-bd01-68ea6ce6adfd.png)

## 1. Mesh topology

In a mesh topology, every device is connected to another device via a particular channel. 

![1-75](https://user-images.githubusercontent.com/42698268/144440132-614bc9cc-943f-4fb5-9a4e-fcfca3bb2238.png)


Figure 1: Every device is connected with another via dedicated channels. These channels are known as links. 
 

* Suppose, N number of devices are connected with each other in a mesh topology, the total number of ports that are required by each device is N-1. In Figure 1, there are 5 devices connected to each other, hence the total number of ports required by each device is 4. Total number of ports required=N*(N-1).
* Suppose, N number of devices are connected with each other in a mesh topology, then the total number of dedicated links required to connect them is NC2 i.e. N(N-1)/2. In Figure 1, there are 5 devices connected to each other, hence the total number of links required is 5*4/2 = 10.

***Advantages of this topology:***

* It is robust.
* The fault is diagnosed easily. Data is reliable because data is transferred among the devices through dedicated channels or links.
* Provides security and privacy.


***Problems with this topology :*** 

* Installation and configuration are difficult.
* The cost of cables is high as bulk wiring is required, hence suitable for less number of devices.
* The cost of maintenance is high.

## 2. Star Topology :
In star topology, all the devices are connected to a single hub through a cable. This hub is the central node and all other nodes are connected to the central node. The hub can be passive in nature i.e., not an intelligent hub such as broadcasting devices, at the same time the hub can be intelligent known as an active hub. Active hubs have repeaters in them. 

![2-49](https://user-images.githubusercontent.com/42698268/144440578-0682bc99-d45e-4722-9a1c-5ed604045323.png)

Figure 2: A star topology having four systems connected to a single point of connection i.e. hub.

***Advantages of this topology :***

* If N devices are connected to each other in a star topology, then the number of cables required to connect them is N. So, it is easy to set up.
* Each device requires only 1 port i.e. to connect to the hub, therefore the total number of ports required is N.


***Problems with this topology :***

* If the concentrator (hub) on which the whole topology relies fails, the whole system will crash down.
* The cost of installation is high.
* Performance is based on the single concentrator i.e. hub.


## [Bus and Ring](https://www.youtube.com/watch?v=7t0YJWTjmdI&list=PLxCzCOWd7aiGFBD2-2joCpWOLUrDLvVV_&index=6)

![Screenshot from 2021-12-02 20-27-10](https://user-images.githubusercontent.com/42698268/144446490-9e9db9d5-4cb2-4ff1-b1a7-8a12f4424962.png)

## 3. Bus Topology

Bus topology is a network type in which every computer and network device is connected to a single cable. It transmits the data from one end to another in a single direction. No bi-directional feature is in bus topology. It is a multi-point connection and a non-robust topology because if the backbone fails the topology crashes.


![3-55](https://user-images.githubusercontent.com/42698268/144447718-94320b11-e961-48f4-808f-80ed6e94317a.png)

Figure 3: A bus topology with shared backbone cable. The nodes are connected to the channel via drop lines. 

***Advantages of this topology :***

* If N devices are connected to each other in a bus topology, then the number of cables required to connect them is 1, which is known as backbone cable, and N drop lines are required.
* The cost of the cable is less as compared to other topologies, but it is used to build small networks.
 
 ***Problems with this topology :***

* If the common cable fails, then the whole system will crash down.
* If the network traffic is heavy, it increases collisions in the network. To avoid this, various protocols are used in the MAC layer known as Pure Aloha, Slotted Aloha, CSMA/CD, etc.
* Security is very low.


## 4. Ring Topology :
In this topology, it forms a ring connecting devices with its exactly two neighboring devices.

A number of repeaters are used for Ring topology with a large number of nodes, because if someone wants to send some data to the last node in the ring topology with 100 nodes, then the data will have to pass through 99 nodes to reach the 100th node. Hence to prevent data loss repeaters are used in the network.
The transmission is unidirectional, but it can be made bidirectional by having 2 connections between each Network Node, it is called Dual Ring Topology.


![4-32](https://user-images.githubusercontent.com/42698268/144448334-0c35ee6d-45ee-4793-9d8a-e542b79b607b.png)

Figure 4: A ring topology comprises 4 stations connected with each forming a ring. 

***The following operations take place in ring topology are :***
 

1. One station is known as a monitor station which takes all the responsibility to perform the operations.
2. To transmit the data, the station has to hold the token. After the transmission is done, the token is to be released for other stations to use.
3. When no station is transmitting the data, then the token will circulate in the ring.
4. There are two types of token release techniques: Early token release releases the token just after transmitting the data and Delay token release releases the token after the acknowledgment is received from the receiver.


***Advantages of this topology :***

* The possibility of collision is minimum in this type of topology.
* Cheap to install and expand.


***Problems with this topology :***

* Troubleshooting is difficult in this topology.
* The addition of stations in between or removal of stations can disturb the whole topology.
* Less secure.


## 5. Tree Topology :
This topology is the variation of Star topology. This topology has a hierarchical flow of data. 


![tree-topology2](https://user-images.githubusercontent.com/42698268/144448768-8bce0be1-602b-4707-8b91-3ca189a6354a.png)


Figure 5: In this, the various secondary hubs are connected to the central hub which contains the repeater. In this data flow from top to bottom i.e. from the central hub to secondary and then to the devices or from bottom to top i.e. devices to the secondary hub and then to the central hub. It is a multi-point connection and a non-robust topology because if the backbone fails the topology crashes.
 

***Advantages of this topology :***

* It allows more devices to be attached to a single central hub thus it decreases the distance that is traveled by the signal to come to the devices.
* It allows the network to get isolate and also prioritize from different computers.


***Problems with this topology :***  

* If the central hub gets fails the entire system fails.
* The cost is high because of cabling.

# L-7 Machester encoding and differential manchester encoding 

## Manchester
![Screenshot from 2021-12-03 16-21-14](https://user-images.githubusercontent.com/42698268/144590932-4b090dd5-4ba2-4512-8375-42f177c4f558.png)

![Screenshot from 2021-12-03 16-21-32](https://user-images.githubusercontent.com/42698268/144590953-ab5d90e7-8813-4c00-96c8-faa088a80979.png)

## Differential Manchester

![Screenshot from 2021-12-03 16-33-55](https://user-images.githubusercontent.com/42698268/144592218-681c0719-c06f-4088-95b2-97492ce765f9.png)






# 3. [Protocol and standard in computer network](https://www.geeksforgeeks.org/protocol-and-standard-in-computer-networks/)

## Protocol :
In Order to make communication successful between devices , some rules and procedures should be agreed upon at the sending and receiving ends of the system. Such rules and procedures are called as Protocols . Different types of protocols are used for different types of communication.


![protocol](https://user-images.githubusercontent.com/42698268/144449657-d28139e8-2a79-40ab-a414-7df2a450f3a7.png)

In above diagrams Protocols are shown as set of rules . Such that Communication between Sender and Receiver is not possible without Protocol.

## Standards : 

Standards are the set of rules  for data communication that are needed for  exchange of information among devices. It is important to follow Standards which are created by various  Standard Organization like IEEE , ISO , ANSI etc.

***Types of Standards :***

Standards are of two types :

* De Facto Standard.
* De Jure  Standard.


***De Facto Standard*** :  The meaning of the work ” De Facto ”  is ” By Fact ”  or “By Convention”.
These are the standard s that have not been approved by any Organization , but have been adopted as  Standards  because of it’s widespread use. Also , sometimes these standards are often established by Manufacturers.

For example :   Apple  and Google are two companies which established their own rules on their products which are different . Also they use some same standard rules for manufacturing for their products.

***De Jure Standard*** :  The meaning of the word “De Jure”  is  “By Law” or “By  Regulations” . 
Thus , these are the  standards that have been approved by officially recognized body like ANSI , ISO , IEEE etc. These are the standard which are important to follow if it is required or needed.

***For example*** :  All the data communication standard  protocols like SMTP , TCP , IP , UDP etc. are important to follow the same when we needed them. 


## protocol vs standard
A protocol defines a set of rules used by two or more parties to interact between themselves. A standard is a formalized protocol accepted by most of the parties that implement it.



# 4. OSI Model

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

# 5. Types of Transmission Media

In data communication terminology, a transmission medium is a physical path between the transmitter and the receiver i.e. it is the channel through which data is sent from one place to another. Transmission Media is broadly classified into the following types:  

![TypesOfTransmissionMedia](https://user-images.githubusercontent.com/42698268/144472452-30feb75c-5b76-4f8c-ab84-8c6d41ca3b74.png)

## 1. Guided Media: 
It is also referred to as Wired or Bounded transmission media. Signals being transmitted are directed and confined in a narrow pathway by using physical links. 

Features:
* High Speed
* Secure
* Used for comparatively shorter distances

There are 3 major types of Guided Media: 

### (i) Twisted Pair Cable –

It consists of 2 separately insulated conductor wires wound about each other. Generally, several such pairs are bundled together in a protective sheath. They are the most widely used Transmission Media. Twisted Pair is of two types: 

* ***Unshielded Twisted Pair (UTP):***

UTP consists of two insulated copper wires twisted around one another. This type of cable has the ability to block interference and does not depend on a physical shield for this purpose. It is used for telephonic applications.


![UntitledDiagram321](https://user-images.githubusercontent.com/42698268/144473822-c530ddd3-9531-4f88-9f3b-675ea45867c1.png)



Advantages: 

⇢ Least expensive

⇢ Easy to install

⇢ High-speed capacity

⇢ Susceptible to external interference

⇢ Lower capacity and performance in comparison to STP

⇢ Short distance transmission due to attenuation


* ***Shielded Twisted Pair (STP):***
This type of cable consists of a special jacket (a copper braid covering or a foil shield) to block external interference. It is used in fast-data-rate Ethernet and in voice and data channels of telephone lines.

![UntitledDiagram331](https://user-images.githubusercontent.com/42698268/144474193-c727d8bf-379a-46f3-95ad-672cbcb0b33b.png)

Advantages: 

⇢ Better performance at a higher data rate in comparison to UTP

⇢ Eliminates crosstalk

⇢ Comparatively faster

⇢ Comparatively difficult to install and manufacture

⇢ More expensive

⇢ Bulky


### (ii) Coaxial Cable – 
It has an outer plastic covering containing an insulation layer made of PVC or Teflon and 2 parallel conductors each having a separate insulated protection cover. The coaxial cable transmits information in two modes: Baseband mode(dedicated cable bandwidth) and Broadband mode(cable bandwidth is split into separate ranges). Cable TVs and analog television networks widely use Coaxial cables. 


![UntitledDiagram72](https://user-images.githubusercontent.com/42698268/144474314-9e21e703-33ff-455d-a770-2436c10a963f.png)

Advantages: 

* High Bandwidth
* Better noise Immunity
* Easy to install and expand
* Inexpensive


Disadvantages:  

* Single cable failure can disrupt the entire network


### (iii) Optical Fiber Cable – 
It uses the concept of reflection of light through a core made up of glass or plastic. The core is surrounded by a less dense glass or plastic covering called the cladding. It is used for the transmission of large volumes of data. 

The cable can be unidirectional or bidirectional. The WDM (Wavelength Division Multiplexer) supports two modes, namely unidirectional and bidirectional mode.


![UntitledDiagram62](https://user-images.githubusercontent.com/42698268/144474491-bb9b9ca4-bdf8-4bad-856b-32d9ccfef530.png)


Advantages:  

* Increased capacity and bandwidth
* Lightweight
* Less signal attenuation
* Immunity to electromagnetic interference
* Resistance to corrosive materials


Disadvantages:  

* Difficult to install and maintain
* High cost
* Fragile

### (iv) Stripline
Stripline is a transverse electromagnetic (TEM) transmission line medium invented by Robert M. Barrett of the Air Force Cambridge Research Centre in the 1950s. Stripline is the earliest form of the planar transmission line. It uses a conducting material to transmit high-frequency waves it is also called a waveguide. This conducting material is sandwiched between two layers of the ground plane which are usually shorted to provide EMI immunity.

### (v) Microstripline

In this, the conducting material is separated from the ground plane by a layer of dielectric.


## 2. Unguided Media: 
It is also referred to as Wireless or Unbounded transmission media. No physical medium is required for the transmission of electromagnetic signals. 

Features:  

* The signal is broadcasted through air
* Less Secure
* Used for larger distances


There are 3 types of Signals transmitted through unguided media: 

* (i) Radio waves – 

These are easy to generate and can penetrate through buildings. The sending and receiving antennas need not be aligned. Frequency Range:3KHz – 1GHz. AM and FM radios and cordless phones use Radio waves for transmission. 


![radiowave3](https://user-images.githubusercontent.com/42698268/144474869-51f4b81b-5f45-45be-bf91-f6ad2007bd8c.png)

Further Categorized as (i) Terrestrial and (ii) Satellite. 


* (ii) Microwaves – 

It is a line of sight transmission i.e. the sending and receiving antennas need to be properly aligned with each other. The distance covered by the signal is directly proportional to the height of the antenna. Frequency Range:1GHz – 300GHz. These are majorly used for mobile phone communication and television distribution. 


![microwave300x81](https://user-images.githubusercontent.com/42698268/144474981-916b8e47-a875-4468-af0f-e8902b1c524f.png)


## (iii) Infrared – 
Infrared waves are used for very short distance communication. They cannot penetrate through obstacles. This prevents interference between systems. Frequency Range:300GHz – 400THz. It is used in TV remotes, wireless mouse, keyboard, printer, etc.


![infrared1](https://user-images.githubusercontent.com/42698268/144475053-b202c768-01e9-438b-a72e-557375ac80f4.png)



# MODULE - 2
![CNmodule2](https://user-images.githubusercontent.com/76476144/144490999-cda91ebc-da3b-4819-ab73-4fae875a8410.jpeg)

# [LAN](https://www.geeksforgeeks.org/local-area-network-lan-technologies/)

Local Area Network (LAN) is a data communication network connecting various terminals or computers within a building or limited geographical area. The connection among the devices could be wired or wireless. Ethernet, Token Ring and Wireless LAN using IEEE 802.11 are examples of standard LAN technologies. 

Ex:- School,Bank,College,etc.

LAN has the following topologies: 
 

* Star Topology
* Bus Topology
* Ring Topology
* Mesh Topology
* Hybrid Topology
* Tree Topology


Ethernet:- 

Ethernet is the most widely used LAN technology, which is defined under IEEE standards 802.3. The reason behind its wide usability is Ethernet is easy to understand, implement, maintain, and allows low-cost network implementation. Also, Ethernet offers flexibility in terms of topologies that are allowed. Ethernet generally uses Bus Topology. Ethernet operates in two layers of the OSI model, Physical Layer, and Data Link Layer. For Ethernet, the protocol data unit is Frame since we mainly deal with DLL. In order to handle collision, the Access control mechanism used in Ethernet is CSMA/CD. 

Manchester Encoding Technique is used in Ethernet. 


## [Wired LAN](https://www.lifewire.com/wired-vs-wireless-networking-816352)

Computer networks for the home and small business use either wired or wireless technology. Wired Ethernet was once the common choice for homes and businesses. However, Wi-Fi and other wireless options are now prevalent in homes, while many businesses still rely on wired networks.


Both methods have advantages over each other, and both represent viable options for home and other local area networks (LANs). We reviewed both technologies to help you decide which is best for your small network.


![Screenshot from 2021-12-02 23-22-23](https://user-images.githubusercontent.com/42698268/144476512-ebdbae32-8c1f-41a1-9ae2-704dcaf7a288.png)


![Screenshot from 2021-12-02 23-23-37](https://user-images.githubusercontent.com/42698268/144476936-85ccd3b9-e949-497c-86a1-7b58f569ce0c.png)


![Screenshot from 2021-12-02 23-23-56](https://user-images.githubusercontent.com/42698268/144476947-aa098749-c9ed-419d-8814-577c462f63b9.png)


![Screenshot from 2021-12-02 23-26-00](https://user-images.githubusercontent.com/42698268/144477085-c6e9f2b1-921f-498b-8cc1-19f85ec45795.png)



![Screenshot from 2021-12-02 23-24-19](https://user-images.githubusercontent.com/42698268/144477109-a07bec1a-eb99-429f-8ce8-532a59d46c29.png)


![Screenshot from 2021-12-02 23-24-26](https://user-images.githubusercontent.com/42698268/144477122-60ae09bc-8c55-4845-a023-259ac23c6b7c.png)

![Screenshot from 2021-12-02 23-24-44](https://user-images.githubusercontent.com/42698268/144477145-e7509194-9749-42dd-a801-2fa4f981da21.png)

# [Difference between LAN and VLAN](https://www.geeksforgeeks.org/difference-between-lan-and-vlan/)
LAN stands for Local Area Network is a group of network devices which allow the communication between connected devices. On the other hand VLAN stands for Virtual Local Area Network which is used to enhance the performance of LANs (Local Area Networks).



![Untitled-Diagram-52](https://user-images.githubusercontent.com/42698268/144560470-d94fb884-d1eb-4960-a1d2-954acc955593.png)

The main difference between LAN (Local Area Network) and VLAN (Virtual Local Area Network) is that LAN work on single broadcast domain on the other hand VLAN works on multiple broadcast domain and In local are network, the Packet is advertised to each device while In virtual local area network, packet is send to specific broadcast domain.

![Untitled-Diagram-44](https://user-images.githubusercontent.com/42698268/144560452-dc844716-2000-433e-a937-3bca85898033.png)

![Screenshot (30)](https://user-images.githubusercontent.com/76476144/144493773-f5481d7e-8d76-4eae-b34d-d3e79a081652.png)

# Techniques of Bandwidth utilization: 

***1. Badwidth overview***
Bandwidth, or precisely network bandwidth, is the maximum rate at which data transfer occurs across any particular path of the network. Bandwidth is basically a measure of the amount of data that can be sent and received at any instance of time. That simply means that higher is the bandwidth of a network, larger is the amount of data network can be sending to and from across its path. Be careful not to confuse bandwidth with closely related terms such as the data rate and the throughput. Bandwidth is something that deals with the measurement of capacity and not the speed of data transfer. 

***2. Units of Measurement :***
Bandwidth is usually measured in bits transferred per second through a path or link. The common units of bandwidth we come across are as follows.

* bps  (Bits per second)
* Mbps (Megabits per second)
* Gbps (Gigabits per second)

***3. What is Bandwidth Utilization?***

Bandwidth utilization can be defined as the amount of bandwidth consumed on a network or network segment and the breakdown of its composite traffic. 


***4. What is Multiplexing***
* Multiplexing is a technique by which different analog and digital streams of transmission can be simultaneously processed over a shared link. Multiplexing divides the high capacity medium into low capacity logical medium which is then shared by different streams.

* Multiplexing refers to multiple sources but one link. In the multiplexing approach, all the devices are connected to MUX and one line to host. The link carries multiple channels of information and the number of lines in it is the same as the number of lines out. 

* Multiplexing is the process of combining multiple signals (analog or digital), commonly from slow devices, onto one very fast communications link. This sharing is achieved by a device called a Multiplexer (MUX) and Demultiplexer (DEMUX). Multiplexing is performed by combining n input lines to generate one output line i.e. (many to one) by using a device called MUX. This means that MUX has several inputs and one output. By a corresponding device, DEMUX, at the other end separating the signal into several subchannels. Therefore, DEMUX has one input and several outputs


![Screenshot from 2021-12-03 13-09-34](https://user-images.githubusercontent.com/42698268/144563951-2f17f797-1836-4c41-88e4-6ea5ad588918.png)



Communication is possible over the air (radio frequency), using a physical media (cable), and light (optical fiber). All mediums are capable of multiplexing.



***5. The different types of Multiplexers:-***

The different types of multiplexers are as follows:
  * A. Frequency Division Multiplexing
  * B. Time Division Multiplexing
  * C. Wavelength Division Multiplexing

   ## A Frequency Division Multiplexing
   Frequency division multiplexing (FDM) is a technique of multiplexing which means combining more than one signal over a shared medium. In FDM, signals of different frequencies are combined for concurrent transmission.
   
   The frequency spectrum is divided into logical channels and each user has exclusive access to the channels, it sends signals into different frequency ranges and carries multiple video channels on a single cable. Every signal is modulated onto separate carrier frequencies which are divided by guard bands. All the assignment for non-overlapping frequency ranges from each user or signal on medium. Therefore, all the signals are transmitted at the same time but through different frequencies. The multiplexer accepts inputs and assigns frequency to each device. 
   
   ### Disadvantages of FDM:
      It has only one drawback that it cannot utilize the full capacity of the cable. 
   
  ## B.  Time Division Multiplexing
   * TDM is applied primarily on digital signals but can be applied on analog signals as well. In TDM the shared channel is divided among its user by means of time slot. Each user can transmit data within the provided time slot only. Digital signals are divided in frames,equivalent to time slot i.e. frame of an optimal size which can be transmitted in given time slot.

   TDM works in synchronized mode. Both ends, i.e. Multiplexer and De-multiplexer are timely synchronized and both switch to next channel simultaneously.
   
   * Time Division Multiplexing is generally used in computer communication and telecommunications. In this, the sharing of channels is accomplished by dividing the available transmission time on a medium among the users.

TDM uses digital signalling instead of dividing the cables into frequency bands. 

There are two types of TDMs:
* ***Synchronous Time Division Multiplexing***: In this, the multiplexer and the de-multiplexer have to decide on time slots. 
* ***Statistical Time Division Multiplexing:*** In this, the time division is fixed.
        
  ## C. Wavelength Division Multiplexing
  * Light has different wavelength (colors). In fiber optic mode, multiple optical carrier signals are multiplexed into an optical fiber by using different wavelengths. This is an analog multiplexing technique and is done conceptually in the same manner as FDM but uses light as signals.
  * WDM is similar to Frequency Division Multiplexing but it is applied to fibers. The only difference between them is that the operating frequencies are much higher than they are in the optical range. It multiplexes multiple data streams onto a single fiber optic line and different wavelength lasers transmit the multiple signals. 

--> It is of two types:

* Dense wavelength division multiplexing: It combines many channels into one fiber.
* Coarse wavelength division multiplexing: It combines fewer channels into one fiber.

      
 # [Spread spectrum](https://www.javatpoint.com/spread-spectrum-in-mobile-computing)
 
## Definition
* Spread spectrum is a form of wireless communications in which the frequency of the transmitted signal is deliberately varied. This results in a much greater bandwidth than the signal would have if its frequency were not varied.
* Spread spectrum is a technique used for wireless communications in telecommunication and radio communication. In this technique, the frequency of the transmitted signal, i.e., an electrical signal, electromagnetic signal, or acoustic signal, is deliberately varied and generates a much greater bandwidth than the signal would have if its frequency were not varied.

In other words, "Spread Spectrum is a technique in which the transmitted signals of specific frequencies are varied slightly to obtain greater bandwidth as compared to initial bandwidth."

Now, spread spectrum technology is widely used in radio signals transmission because it can easily reduce noise and other signal issues.
  
  
## Reasons to use Spread Spectrum
* Spread spectrum signals are distributed over a wide range of frequencies and then collected and received back to the receiver. On the other hand, wide-band signals are noise-like and challenging to detect.
* Initially, the spread spectrum was adopted in military applications because of its resistance to jamming and difficulty intercepting.
* Now, this is also used in commercial wireless communication.
* It is most preferred because of its useful bandwidth utilization ability.
 
 
## Usage of Spread Spectrum
There are many reasons to use this spread spectrum technique for wireless communications. The following are some reasons:

* It can successfully establish a secure medium of communication.
* It can increase the resistance to natural interference, such as noise and jamming, to prevent detection.
* It can limit the power flux density (e.g., in satellite down links).
* It can enable multiple-access communications.

## Types of Spread Spectrum
Spread Spectrum can be categorized into two types:

* Frequency Hopping Spread Spectrum (FHSS)
* Direct Sequence Spread Spectrum(DSSS)


![spread-spectrum](https://user-images.githubusercontent.com/42698268/144565824-3fc7616d-25cf-4a62-b9a8-23c73f6e8953.png)




# MODULE 3

![Screenshot from 2021-12-03 13-24-47](https://user-images.githubusercontent.com/42698268/144565995-96e57970-d25f-4f4f-9c94-8de8f972de3f.png)



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




# L-8 Various Network devices


![Screenshot from 2021-12-03 17-36-23](https://user-images.githubusercontent.com/42698268/144614854-ddd18fbb-84d0-46e0-b721-51c8563ab802.png)

## 1. [Cables](https://www.computernetworkingnotes.com/networking-tutorials/network-cable-types-and-specifications.html)
To connect two or more computers or networking devices in a network, network cables are used. There are three types of network cables; coaxial, twisted-pair, and fiber-optic.


![Screenshot from 2021-12-03 20-02-21](https://user-images.githubusercontent.com/42698268/144621636-46ad8048-7fe8-447c-8266-4470e38b93a1.png)

![Screenshot from 2021-12-03 20-11-20](https://user-images.githubusercontent.com/42698268/144621658-a3fd586e-691d-454f-8b0a-2fafbda0c2a7.png)

***A. Coaxial cable***

This cable contains a conductor, insulator, braiding, and sheath. The sheath covers the braiding, the braiding covers the insulation, and the insulation covers the conductor.

![nt12-01-coaixal-cable](https://user-images.githubusercontent.com/42698268/144622023-baf35a0c-361c-40de-aa37-00f55dfbf01e.png)

* *Sheath*: This is the outer layer of the coaxial cable. It protects the cable from physical damage.

* *Braided shield*: This shield protects signals from external interference and noise. This shield is built from the same metal that is used to build the core.

* *Insulation*: Insulation protects the core. It also keeps the core separate from the braided shield. Since both the core and the braided shield use the same metal, without this layer, they will touch each other and create a short-circuit in the wire.

* *Conductor*:The conductor carries electromagnetic signals. Based on conductor a coaxial cable can be categorized into two types; single-core coaxial cable and multi-core coaxial cable.


![nt12-02-single-core-multi-core-coaxial-cable](https://user-images.githubusercontent.com/42698268/144622293-dfbab7b8-3f23-4957-bb94-5c7315c6c657.png)




***B. Twisted-pair cables***

The twisted-pair cable was primarily developed for computer networks. This cable is also known as Ethernet cable. Almost all modern LAN computer networks use this cable.

This cable consists of color-coded pairs of insulated copper wires. Every two wires are twisted around each other to form pair. Usually, there are four pairs. Each pair has one solid color and one stripped color wire. Solid colors are blue, brown, green, and orange. In stripped color, the solid color is mixed with the white color.

Based on how pairs are stripped in the plastic sheath, there are two types of twisted-pair cable; UTP and STP.

In the UTP (Unshielded twisted-pair) cable, all pairs are wrapped in a single plastic sheath.

In the STP (Shielded twisted-pair) cable, each pair is wrapped with an additional metal shield, then all pairs are wrapped in a single outer plastic sheath.

**Similarities and differences between STP and UTP cables**
* Both STP and UTP can transmit data at 10Mbps, 100Mbps, 1Gbps, and 10Gbps.
* Since the STP cable contains more materials, it is more expensive than the UTP cable.
* Both cables use the same RJ-45 (registered jack) modular connectors.
* The STP provides more noise and EMI resistance than the UTP cable.
* The maximum segment length for both cables is 100 meters or 328 feet.
* Both cables can accommodate a maximum of 1024 nodes in each segment.


![nt12-03-stp-utp-cables](https://user-images.githubusercontent.com/42698268/144622564-f7e9bb7e-c004-432b-84d9-0e4846d00a4c.png)


***C. Fiber optic cable***

This cable consists of a core, cladding, buffer, and jacket. The core is made from thin strands of glass or plastic that can carry data over a long distance. The core is wrapped in the cladding; the cladding is wrapped in the buffer, and the buffer is wrapped in the jacket.

* Core carries the data signals in the form of light.
* Cladding reflects light back to the core.
* Buffer protects the light from leaking.
* The jacket protects the cable from physical damage.


Fiber optic cable is completely immune to EMI and RFI. This cable can transmit data over a long distance at the highest speed. It can transmit data up to 40 kilometers at the speed of 100Gbps.

Fiber optic uses light to send data. It reflects light from one endpoint to another. Based on how many beams of light are transmitted at a given time, there are two types of fiber optical cable; SMF and MMF.

![nt12-04-smf-mmf-fiber-optical](https://user-images.githubusercontent.com/42698268/144622761-c4e802c2-d870-4a9d-b034-97aac4bb05df.png)

**SMF (Single-mode fiber) optical cable**

This cable carries only a single beam of light. This is more reliable and supports much higher bandwidth and longer distances than the MMF cable. This cable uses a laser as the light source and transmits 1300 or 1550 nano-meter wavelengths of light.

**MMF (multi-mode fiber) optical cable**

This cable carries multiple beams of light. Because of multiple beams, this cable carries much more data than the SMF cable. This cable is used for shorter distances. This cable uses an LED as the light source and transmits 850 or 1300 nano-meter wavelengths of light.

That’s all for this tutorial. If you like this tutorial, please share it with friends via your favorite social networking sites and subscribe to our YouTube channel.

## 2. Repeater – 
A repeater operates at the physical layer. Its job is to regenerate the signal over the same network before the signal becomes too weak or corrupted so as to extend the length to which the signal can be transmitted over the same network. An important point to be noted about repeaters is that they do not amplify the signal. When the signal becomes weak, they copy the signal bit by bit and regenerate it at the original strength. It is a 2 port device. 

![Screenshot from 2021-12-03 20-33-47](https://user-images.githubusercontent.com/42698268/144624625-092a8c29-d6e7-4736-b9c7-188d4b6f5186.png)

## 2. Hub – 


![Screenshot from 2021-12-03 22-35-51](https://user-images.githubusercontent.com/42698268/144643634-f099051e-c1d5-4fb1-b86e-1e25ae076081.png)


![Screenshot from 2021-12-03 22-36-52](https://user-images.githubusercontent.com/42698268/144643643-c1c89dde-2a18-461a-be40-26bd713d1399.png)



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




# [COMPUTER NETWORK NOTES](https://www.computernetworkingnotes.com/networking-tutorials/)



