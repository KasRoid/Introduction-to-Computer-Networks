# Understanding Switches

## Refresher on Switches

- Connects devices together just like a hub
- Intelligent network device (OSI Layer 2)
- Memorizes the **MAC Address** of each device connected to it via **MAC Address Talbe**
  - Pays attention to source and destination MAC addresses during communication process.
- Breaks up collision domains
  - Traffic goes in one port and is repeated out to only destination port
  - Standard in today's network infrastructure

---

## Collision Domains

### Understanding Collision Domains

- A Collision domain is simply a network segment in which data collisions can occur.
- Collisions can occur on ethernet networks using:
  - Hubs
  - Switches in Half-Duplex Mode
- We utilize CSMA/CD to help minimize collisions
  - Carrier Sense Multiple Access with Collsion Detection

**Hubs**
Create one large collision domain.

![HUbs Image](Hubs.png)

**Switches (Half-Duplex)**
Break collision domains up into smaller ones.

![Switches Image](Switches.png)

### Full Duplex Switches Eliminate Collision

- Collisions don't occur on switches utilizing full duplex mode:
  - There's dedicated channel for concurrent sending and receiving data.

![Full Duplex Swithces](Full-Duplex-Swithces.png)

---

## Understanding Broadcast Domains

A broadcast domain is a network segment in which all devices on that network receive ethernet broad casts messages(one-to-all) from each other.

- Example Broadcast Protocols: ARP, DHCP

Hubs and switches forward broadcast messages; routers do not.

- Broadcast messages are very inefficient and resource-intensive.
- If routers allowed broadcasts, WAN and Internet performance would drastically decline due to boradcast storms.

![Broadcast Domains](Broadcast-Domains.png)

---

## CSMA/CD

- Carrier Sense Multiple Access with Collsion Detection
- Used ona shared network meduim to help reduce data collisions.
- Helps hosts decide when to send data and also detect collisions
- Used with hubs(multi-port repeaters)
- Used with switches ONLY in half-duplex mode.

**CSMA/CD Process**
![CSMA/CD Process Image](CSMA-CD-Process.png)

---

## Unmanaged vs. Managed switches

### Unmanaged

- Completely unmanaged.
- Unbox it, plug it in, and it works without any administration.

### Managed

- Can be configured and managed by network administrators, typically via Telnet or SSH.
  - Configure static entries in the MAC table.
  - Configure half or full-duplex on specific ports.
  - Monitor switch performance with SNMP.
  - Create virtual LANs(VLANs)
  - Configure Port Mirroring
- Much more expensive than unmanaged switches.
