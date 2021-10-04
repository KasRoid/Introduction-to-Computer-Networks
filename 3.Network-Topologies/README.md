# Network Topologies

**Physical Topologies**
Describe the placement of network devices and how they are physically connected

**Logical Topologies**
Describe how data flows throughout a network

## Wired Network Topologies

Four Specific Topologies

- Bus
  - All Devices are connected to a single coaxial network cable.
    - Devices are connected via a vampire tap or T-Connector.
    - Terminators are required at both ends of the cable to prevent signal bounce.
    - Antiquated technology.
  - Only one end device can be active on network at a time.
    - Data signals travel in both directions and are received by all devices on the network.
  - A single break in the cable can take down the entire network.
- Ring
  - All devices are connected in a circular fashion.
  - Each computer is connected to two other computers.
  - Data travles from node-tonode with each computer handling data, either unidirectional or bidirectional.
  - Each device(node) in the ring regenerates the signal, acting as a repeater.
  - Failure of a singl enode can take down the entire network.
  - Fiber Distributed Data Interface (FDDI) uses two counter-rotating ring topologies for redundancy.
- Star
  - All devices are connected to a central connecting device, which is usually a switch.
  - Devices send data to the switch, which forwards it to the appropriate destination device.
  - Popular topology in today's networks.
  - Used in most large and small Networks
  - Central device is a single point of failure.
- Mesh
  - Each device is connected to every other device by separate cabling.
  - Highly redundant and fault-tolerance.
  - Expensive to install
  - Commonly used in Enterprise Networks & WANs.
  - Two Types
    - Partail Mesh
    - Full Mesh

## Wireless Network Topologies

Wireless networks utilize radio frequencies(RF) to communicate.

Three Specific Topologies

- Ad hoc
  - Peer-to-Peer(P2P) wireless network where no wireless access point(WAP) infrastructure exits.
  - The devices communicate directly with one another.
  - Personal area networks(PANs) are a common example of Ad hoc wireless networks.
- Infrastructure
  - Wireless network that uses wireless access point(WAP) as it's central connecting device.
  - Infrastructure wireless networks(WLANs) a commonly used in homes and small offices.
- Mesh
  - Just like a wired mesh design, wireless mesh networks utilizes several wireless access points(nodes) to create a robust wireless network that is
    - Scalable
    - Self-Healing
    - Reliable(redundancy)
  - Common in larger homes and businesses
