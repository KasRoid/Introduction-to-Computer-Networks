# IP Addressing Version 6

## Disadvantages of IPv4

- Not enough IPv4 Addresses
  - Approximately 4.3 billion public IP addresses
  - 7.8 billion world population
  - Multiple devices per user (computers, tablets, smart phones, smart TVs, home automation, etc.)
- Less Efficient Routing (compared to IPv6)
- Security is Optional
  - Encrypted data is optional

## IPv6 Solutions

- Plethora of Addresses
  - 128-bit binary address space compared to 32-bit for IPv4
  - 340 trillion trillion trillion addresses
  - 5 x 10^28 addresses for each person on the planet
- Simplified Internet Routing Tables
  - IPv6 packet header enables more efficient routing
    - Fixed at 40 Bytes versus IPv4 "Variable Length" Packet Header for Optional Fields
- Easier & Automated Configuration Compared to IPv4
  - Stateless Auto-Configuration
  - No need for a DHCP server
- Security is Required
  - Internet Protocol Security (IPSec) is required.
    - Source IP can be authenticated
    - Data in transit is encrypted

## IPv4 vs. Ipv6

|                     | IPv4        | IPv6      |
| ------------------- | ----------- | --------- |
| Deployed            | 1981        | 1999      |
| Address Size        | 32-Bit      | 128-Bit   |
| Number of Addresses | 2^32        | 2^128     |
| Addressing          | Class-Based | Classless |

## Why is IPv4 Still Around?

- Subnetting / CIDR
- Use of Private IP Addresses
- Network Address Translation(NAT)

---

## IPv6 Addressing

- 128-bit address composed of eight 16-bit hexadecimal blocks, separated by colons
- Each number of letter is 4 binary bits.
- They are shown in hexadecimal to simply the address
  - 128 digits in binary format
  - Up to 64 digits in decimal format.
- Example
  - Hexadecimal: 85A3
  - Binary: 1000 0101 1010 0011
  - Decimal 8 5 10 3

## The Network and Interface IDs

![IPv6 Image](IPv6.png)

- 128-bit address composed of eight 160bit Hexadecimal blocks, separated by colons.
- Network ID
  - Site Prefix: Used for routing over the Internet
  - Subnet ID: Used for subnets on internal networks.
- Interface ID
  - The host portion of the adress, that's automatically configured from the MAC address or manually configured in EUI-64 format.

## IPv6 Address Simplification

- We can simplify by omitting leading 0's
  - 0DB8 -> DB8
  - 0000 -> 0
- Can also compress contiguous blocks of 0's into double colon "::" once per address.
  - :0000:0000: -> ::

## IPv6 CIDR

- We can use CIDR notation with IPv6 addresses, similar to IPv4
  - FE80::8A:0:8398:85A3/64
- This telss us
  - Network ID(64-bits): FE80:0000:0000:0000
  - Interface ID(64-biys): 008A:0000:8398:85A3
- A standard IPv6 subnet can have 2^64 IPv6 addresses

---

## IPv6 Transmission Types

- Unicast (One-to-One) Communication
  - One-to-One communication, just like with IPv4
- Multicast (One-to-Many) Communication
  - IPv6 doesn't use broadcast transmissions (one-to-all).
  - IPv6 multicast replaced broadcast communications.
  - Sends to multi-cast group members.
- Anycast (One-to-One-of-Many) Communication
  - Identifies multiple interfaces, but a packet of data is delivered to the nearest network interfaces (used in routing)

---

## Types of IPv6 Addresses

### IPv6 Unicast (One-to-One) Addresses

- Global Addresses
  - Similar to Public IPv4 Addresses
  - Globally Routable over the Internet
  - 2000 Prefix
- Unique Local Addresses
  - Similar to Private IPv4 Addresses
  - Internally routable, but not routable over the Internet
  - FC00 or FD00 Prefix
- Link-Local Addresses
  - IPv6 Equivalent to IPv4 APIPA Addresses
  - Can be assigned automatically or statically.
  - Not routable internally or over the Internet
  - FE80 Prefix

### IPv6 loopback Addresses

- ::1

---

## IPv4 to IPv6 Translation & Compatibility

### IPv4 to IPv6 Transition

- IPv6 is not natively backward compatible with IPv4
- To aid in the transition, as well as to allow IPv4 and IPv6 to co-exist, there are two transition technologies you need to know
  - Dual IP Stack
  - Tunneling

### IPv4 to IPv6 Compatibility

- Dual IP Stack
  - When both IPv4 and IPv6 protocols co-exist within an operating system.
  - Can be used independently or together.
- Tunneling
  - Tunneling is when we encapsulate IPv4 into IPv6 data and vice versa
    - 4to6
    - 6in4
    - Teredo
    - Miredo

### Tunneling Protocols

- 4to6
  - Encapsulates IPv4 data into an IPv6 Tunnel
- 6in4
  - Encapsulates IPv6 data into an IPv4 Tunnel and can traverse IPv4 NAT.
- Teredo
  - Microsoft Windows IPv6 tunneling protocol similar to 6in4 that supports NAT.
- Miredo
  - A Linux and Unix-based open-source version of Teredo.

---

## IPv6 Neighbor Discovery Protocol (NDP)

- Neighbor Solicitation and Advertisement
  - When an IPv6-enabled system joins a network, it sends out a multicast "neighbor solicitation" to all other IPv6 Systems.
  - All other IPv6 systems on the network will respond with a "neighbor advertisement."
