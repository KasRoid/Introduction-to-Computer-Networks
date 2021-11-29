# Wide Area Networking

## WAN Connection Types

- WAN connections can be broken up into three different categories:
  - Circuit-Switched Connections
  - Packet-Switched Connections
  - Dedicated Leased Lines

### Circuit-Switched Connection

- Designed in 1878, was originally designed for telephone calls.
- Uses a dedicated point-to-point connection (circuit) using a telecommunications network.
  - Creates a dedicated link with fixed bandwidth between communicating nodes.
  - Others can't utilize the circuit during the connection, which may waste bandwidth.
  - Transmissions are sent and received in order, unlike with packet switching, where they can arrive out of order.
- Examples:
  - Dedicated Leased-Lines & Dial-Up

### Packet-Switched Connection

- Data is broken into packets, which are routed to different links to the other endpoint.
- The path varies based on the best route at the time the data is sent.
  - Packets may arrive out of order and must be re-assembled in the correct order.
- Unlike circuit switching, packet switching shares bandwidth and connections with others.
- This method of data transmission is the core technology for the Internet and most LANs.
- Packet-switched connections can create virtual circuits.

### Virtual Circuit

- Connection-oriented packet-switched connections create virtual cicuits.
  - A means of forwarding packets of data in such a way that it appears as if there is a dedicated physical link(circuit) between the source and destination.
- Virtual circuits allow service providers to offer better QoS based on a service level agreement(SLA).
- There a re two types:
  - Permanent Virtual Circuit (PVC: Always Exists
  - Switched Virtuall Circuit (SVC): Considered On-Demand

### Dedicated Leased Line

- Like its name implies, it's a dedicated leased line.
- Commonly called a Point-to-Point link.
- A reserved circuit that provides a fixed bandwidth point-to-point data connection, usually between two offices.
  - It's always active and provides a guaranteed bandwidth for a fixed monthly fee.
- The leased line may be a dedicated physical line or a permanent virtual circuit.
