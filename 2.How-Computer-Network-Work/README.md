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

![Image of OSI Model](OSI-Model.png)

## The TCP/IP Model

- The TCP/IP uite is the most common used protocol suite in which the Internet was built.
- It is essentially the protocol suite in which the Internet was built.
- It is the standard for computer networking.
- It is based ona 4-layer model that is similar to the OSI model.

![Image of TCP/IP Model](TCPIP-Model.png)

## TCP/IP vs. OSI Models

![Image of TCP/IP Model](TCPIP-vs-OSI.png)

---

## MAC Addresses

**Media Access Control(MAC)**
Physical address of the network adapter card

- OSI Layer 2 (Data Link) Layer Address
- TCP/IP Layer 1 (Network Interface) Layer Address
- Six bytes (48 bits), Usually Represented Hexadecimal
  - First three bytes (24bits) are assigned by the IEEE to the manufacturer
    - Organizationally Unique Identifier(OUI) assigned by IEEE(ex: Dell or HP)
  - Last three bytes (24 bits) are usually assigned sequentially
    - Unique Numbers
- 2^24 = 16.7 Million Unique Addresses
