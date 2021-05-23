# Socket.io

*What is packets?*
Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully

1. What is the benefit of transforming data into packets?
to make sure that all segments deliveres successfully.

2. UDP is often refereed to as a connectionless protocol. Why is this?
   *connectionless protocol* : communication between two network endpoints without a prior arrangement in which one network endpoint simply sends a message to the other ,is an alternative type of data transmission in which a network endpoint sends an IT signal automatically, without determining whether a receiver exists or stands ready to receive it.
   *Why is this? (User Datagram Protocol)* : fast, for streaming data(video, audio),there is no beginning, middle, or end to the conversation. Data simply begins to flow between the two systems, use of the UDP protocol is DNS queries. When you attempt to use your Web browser to access www.syngress.com, it must first resolve the name to an IP address. This would require a DNS query. The query is sent over a single UDP packet. The DNS server would then respond by telling the originating system the IP address of the Web server. Because the UDP response is faster than setting up a TCP session, UDP makes sense in these situations.

3. Can a socket server application have multiple socket connections? yes

4. Can a socket connection application be connected to multiple socket servers? No

5. Can an application be both a socket server and a socket connection? I don't think so

**TERMS:**

*Observer Pattern:* is used when there is one-to-many relationship between objects such as if one object is modified, its depenedent objects are to be notified automatically. Observer pattern falls under behavioral pattern category.uses three actor classes. Subject, Observer and Client.

*Listener:* function in a computer program that waits for an event to occur.

*Event Handler:* response function for an event

*Event Driven Programming:* flow of the program is determined by events such as user actions

*Event Loop:* is a programming construct or design pattern that waits for and dispatches events or messages in a program.

*Event Queue:* is responsible for sending new functions to the track for processing. It follows the queue data structure to maintain the correct sequence in which all operations should be sent for execution.

*Call Stack:* is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function

*Emit/Raise/Trigger:* fire the event

*Subscribe:* gives us the ability to separate different module/component from each other and send/receive messages from them without any tightly coupled relation or even needing to know about each other.Such as promises

*database:* is an organized collection of data, generally stored and accessed electronically from a computer system. Where databases are more complex they are often developed using formal design and modeling techniques.

-------------------------------------------------------------------------

## OSI Model (Open System Interconnection Model)

- introduce by (ISO)
- Layers :
  - Application Layer
    - used by Network Applications, computer applications that used internet , such as google chrome,FireFox or Skype
    - they use HTTP, HTTPS protocols
    - There are many protocols used in application layer to file transfer(FTP), web surfing(HTTP) ,sending emails(SMTP) or virtual terminals(Telent)

  - Presentation Layer
    - recieves data from Application Layer
    - Translation: convert this data into machine language (01s)
    - Data Compression: reduce the data size
    - Encryption: Encrypt the data using (SSL)

  - Session Layer
    - setting up and manage connections
    - sending and recieving data
    - APIs / NETBIOS
    - Authentication
    - Authorization
    - keep tracking on the data that have been downloaded(images/Texts)

  - Transport Layer
    - controls the reliability of communication
    - segmentation
    - Flow control : ammount of the data that have been transmitted
    - Error control : if some data doesn't arrive the destination (TCP)/(UDP)
    - connection-oriented transmission => (TCP)
    - connectionless transmission => (UDP)
    - UDP is faster than TCP because UDP doesn't  provide any feedback
    - UDP using when it doesn't matter if data recieved or not , like movies , songs or games
    - TCP used when deliver data is must

  - Network Layer
    - data unit are called packets
    - Logical Addressing : IPv4, IPv6 assigned to each data package to arrive to the correct destination
    - Path determination: choose the best path from the source to destination to data delivery(OSPF/BGP / IS-IS)
    - Routing: move the data packets drom source to destination based on IP address and mask

  - Data Link Layer:
    - recieve data packets from network layer
    - Logical addressing: done at network layer (IP address for sender and reciever)
    - Physical addressing : donw at data-link layer (MAC adresses for sender and reciever)
    - trnsform data frome computer to another using local media(wire, wireless)
    - allow upper layers to access media using framing
    - controls how data is placed and recieved from the media (Media Access Control & Error Detection)

  - Physical Layer
    - convert the packet into (01s) format to convert it to the signals

- each layer is a package of protocols

-------------------------------------------------------------------------

## TCP - Three-way handshake

- **TCP** : stands for transmission control protocol
- reliable and connection-oriented transport protocol
- suppose a client wants to get web pages from a server, Before any data transmission , TCP must be established first through 3-wat handshake
- The client sends a SYN(sync) segment to the server, asking for sync(connection)
- The server replies with SYN-ACk (sync, Acknowlegment)
- The server acknowledged the client's connection request, asks the client to open a connection too
- The client replies with ACK(yes)
- Then the two-way connection is established between them

**WebSocket :**
> is a computer communications protocol, providing full-duplex communication channels over a single TCP connection

**Socket.io:** is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of

> Socket.IO enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. Socket.IO is built on top of the WebSockets API (Client side) and Node.js. It is one of the most depended upon library on npm (Node Package Manager)

**How does that work?**

- The client will try to establish a WebSocket connection if possible, and will fall back on HTTP long polling if not.

*WebSocket* is a communication protocol which provides a full-duplex and low-latency channel between the server and the browser. More information can be found here.

So, in the best-case scenario, provided that:

- the browser supports WebSocket (97% of all browsers in 2020)
- there is no element (proxy, firewall, …) preventing WebSocket connections between the client and the server

- sever API

```
const io = require("socket.io")();
// or
const { Server } = require("socket.io");
const io = new Server();

```

- client API : Exposed as the io namespace in the standalone build, or the result of calling `require("socket.io-client")` .