# Network Devices

Network Interface Card(NIC)

- Provides the physical and electrical, light or radio frequency connections to the network media.
- It can either be an expansion card, USB devices or built directly into the motherboard.

Hubs

- Used to Connect Devices Together Within a Network
- Used in Early Networks; Replaced by switches
- Multi-Port repeater
  - Traffic goes in one port and is repeated(broadcatsed) out every other port
  - OSI Layer 1 Device
  - Dumb Network Device
  - Causes increased network collision errors
- Much Less Efficient than a switch
- Legacy Equipment No Longer Used

Switches

- Connects Devices Together Just Like a Hub
- Intelligent Network Device (OSI Layer 2)
- Memorizes the MAC Address of each device connected to it via a MAC Address Table, sometimes called a content Addressable Memory(CAM) Table
- Pays attention to source and destination MAC addresses during communication process
- Use Application-Specific Integrated Circuitry(ASIC), which makes them extremely fast
- Breaks up collision domains
  - traffic goes in one port and is repeated out to only destination port
  - designed for high bandwidth
  - standard in today's network infrastructure

Wireless Acess Points(WAP)

- A wireless access point is a bridge that extends the wired network to the wireless network.
- Just like a switch, it's a Data Link Layer 2 device.
- A WAP is not a router.

Wireless Range Extenders

- Extends the range of a wireless network by acting as a wireless repeater.
- Rebroadcasts radio frequencies from the wireless network it is associated with.

Routers

- Used to connect different networks together
- Routes traffic between networks using IP Addresses
- Uses intelligent decisions(Routing Protocols) to find the best way to get a packet of information from one network to another
- Break up broadcast domains
- OSI Layer 3 device
  - Layer 3 = Router
  - Layer 2 = Switch
  - Layer 1 = Hub

Modems

- Modems modulate one signal to another, such as analog to digital
- For example, modulating a telephone analog signal into a digital signal that a router cna understand

Small Office Home Office(SOHO) Device

- All-in-One wireless router with expanded capabilities
  - router, wireless access point, firewall, switch, DHCP Server, NAT Device, file server, etc.

Media Converters

- Like it's name implies, it converts one media type to another
- Layer 1 Device: performs physical layer signal conversion.
- Ethernet to fiber optic media converters are commonly used.

Firewalls

- The foundation of a defense-in-depth network security strategy
- They protects your network from malicious activity on the Internet
- Prevent unwanted network traffic on different networks from accssing your network.
- Firewalls do this by filtering data packets that go through them.
- They can be a standalone network device or software on a computer system, meaning network-based(hardware) or host-based(software)

Types of Firewalls

- Packet Filtering Firewalls
  - 1st Generation & most Basic
  - Basic filtering rules
- Circuit-Level Firewalls
  - 2nd Generation
  - Monitors valid/invalid TCP Sessions
- Application Layer 7 (NGFW) Firewalls
  - 3rd Generation
  - Much more advanced

DHCP Servers

- Dynamic Host Configuration Protocol Server
- Automatically assigns IP addresses to hosts
- Makes administering a network much easier
- An alternative is static IP addressing

Voice over IP(VoIP) Endpoints

- Most phone systems run over IP networks via dedicated protocols, such as the Session Initiation Protocol(SIP), both in home and office environments.
- VoIP endpoints devices are hardware devices(phones) or software, such as Cisco Jabber that allow you to make phone calls.
