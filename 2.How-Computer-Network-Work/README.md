# How Computer Networks Work

## Computer Networking Protocols

Computers communicate with each other with network protocols. Protocols are rules governing how machines exchange data and enable effective communication.

- Examples
  - When you call somebody, you pick up the phone, ensure there is a dial tone, and if there is, you dial the number.
  - When you drive your car, you obey the rules of the road.

**Physical Protocols**
Describe the medium(wiring), the connections(RJ-45 port), and the signal(voltage level ona wire).

**Logical Protocols**
Software controlling how and when data is sent and received to computers, supporting physical protocols.

Computer networks depend on many different types of protocols in order to work properly.

- Example Common TCP/IP Suite of Protocols
  - Web communication: HTTP
  - E-mail: POP3, SMTP, IMAP
  - File Transfers: FTP

---

## The OSI Model

The Open Systems Interconnection(OSI) Reference Model

- A conceptual framework showing us how data moves throughout a network.
- Give us a guide to understand how networks operate.
- It is not implemented in the real world, TCP/IP is.

## OSI Model Stack

The OSI Model breaks down the complex task of computer-to-computer network communications into 7 layers.

**Upper Layers(Host Layers)**
Handled by the host computer and performs application-specific functions, such as data formatting, encryption, and connection management.

**Lower Layers(Media Layers)**
Provide network-specific functions, such as routing, addressing, and flow control.

![Image of OSI Model](/2.How-Computer-Network-Work/OSI-Model.png)
