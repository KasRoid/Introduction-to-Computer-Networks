# Introduction to Subnetting

## Why Subnet?

- Using default Class A, B and C subnets (called Classful IP Addressing) is inefiicient
  - Wastes unused IP Addresses (Public IP Addresses)
- Allows you to create multiple logical networks that exist withina single Class A, B, or C network.
  - Breaks up larger networks into multiple smaller sub-networks, which are called subnets
- Allows for more efficient routing via router summarization.
- Increased network security!

### Process of Subnetting

- We borrow host bits to create more sub-networks(subnets) from a Class A, B, or C network.
- When you borrow hosts bits
  - You create additional sub-networks, i.e., subnets
  - You also decrease the amount of host IP addresses available to use.

### How to Create Subnets

- Borrow bits from the host portion of an IP address
  - Each bit we borrow is equal to 2^1 Subnets
    - Borrow 1 Host Bit = 2^1 = 2
    - Borrow 2 Host Bits = 2^2 = 4
    - Borrow 3 Host Bits = 2^3 = 8
    - Borrow 4 Host Bits = 2^4 = 16
    - Etc.

![Creating Subnets Visualized Image](Creating-Subnets-Visualized.png)

### Subnetting Questions

- To Create a Subnet, Answer the Floowing Questions
  - How may subnets are needed?
  - How may hosts do you need per subnet?

### Class C Possible Subnets

| Binary (N.N.N.H) | Decimal         | CIDR | # Subnets (2^x) | Block Size (2^y) | # Hosts (2^y - 2) |
| ---------------- | --------------- | ---- | --------------- | ---------------- | ----------------- |
| N.N.N.00000000   | 255.255.255.0   | /24  | 2^0 = 1         | 2^8 = 256        | 2^8 - 2 = 254     |
| N.N.N.10000000   | 255.255.255.128 | /25  | 2^1 = 2         | 2^7 = 128        | 2^7 - 2 = 126     |
| N.N.N.11000000   | 255.255.255.192 | /26  | 2^2 = 4         | 2^6 = 64         | 2^6 - 2 = 62      |
| N.N.N.11100000   | 255.255.255.224 | /27  | 2^3 = 8         | 2^5 = 32         | 2^5 - 2 = 30      |
| N.N.N.11110000   | 255.255.255.240 | /28  | 2^4 = 16        | 2^4 = 16         | 2^4 - 2 = 14      |
| N.N.N.11111000   | 255.255.255.248 | /29  | 2^5 = 32        | 2^3 = 8          | 2^3 - 2 = 6       |
| N.N.N.11111100   | 255.255.255.252 | /30  | 2^6 = 64        | 2^2 = 4          | 2^2 - 2 = 2       |

**Number of Subnets (2^x)**
X = number of host bits we borrow to create subnets

**Block Size (2^y)**
Y = number of remaining host bits left that are used for the subnet IP addresses

**Hosts per Subnets (2^y - 2)**
There are two addresses per network (or subnet) that we cannot use to assign to hosts on that network

- Network Address: This is the address used to uniquely identify the network(or subnet).
- Broadcast Address: Address reserved for broadcast communication on the network.

---

## Subnetting a Class C Network #1

- Details & Requirements
  - Network Address: 192.168.1.0
  - Default Subnet Mask: 255.255.255.0
  - Requires 2 Subnets
- How many host bit do we need to borrow?
  - 1 host bit, 2^1 = 2 Subnets
- How many addresses hosts per subnet?
  - 7 host bits left, 2^7 = 128 Addresses / Subnet
  - 2^7 - 2 = 126 Addresses / Subnet
- What are the valid subnets?
  - 192.168.1.0 and 192.168.1.128
- New Subnet Mask?
  - 11111111.11111111.11111111.10000000
  - 255.255.255.128 or /25

| Subnet            | #1            | #2            |
| ----------------- | ------------- | ------------- |
| Network Address   | 192.168.1.0   | 192.168.1.128 |
| First Host IP     | 192.168.1.1   | 192.168.1.129 |
| Last Host IP      | 192.168.1.126 | 192.168.1.254 |
| Broadcast Address | 192.168.1.127 | 192.168.1.255 |

## Subnetting a Class C Network #2

- Details & Requirements
  - Network Address: 192.168.1.0
  - Default Subnet Mask: 255.255.255.0
  - Requires 4 Subnets
- How many host bit do we need to borrow?
  - 2 host bit, 2^2 = 4 Subnets
- How many addresses hosts per subnet?
  - 6 host bits left, 2^6 = 64 Addresses / Subnet
  - 2^6 - 2 = 62 Addresses / Subnet
- What are the valid subnets?
  - 192.168.1.0, 192.168.1.64, 192.168.1.128 and 192.168.1.192
- New Subnet Mask?
  - 11111111.11111111.11111111.11000000
  - 255.255.255.192 or /26

| Subnet | Network/Subnet Address | Host IP Addresses | Broadcast Address |
| ------ | ---------------------- | ----------------- | ----------------- |
| 1      | 192.168.1.0            | 1 thru 62         | 192.168.1.63      |
| 2      | 192.168.1.64           | 65 thru 126       | 192.168.1.127     |
| 3      | 192.168.1.128          | 129 thru 190      | 192.168.1.191     |
| 4      | 192.168.1.192          | 193 thru 254      | 192.168.1.255     |
