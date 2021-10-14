# A-Deeper-Dive-into-IPv4-Addresses-and-Subnet-Masks

## IP Address Classification and Subnet Mask

### IPv4 Address Classes(Simplified)

| Class | Network Bits | Host Bits |        Address Range        |
| :---: | :----------: | :-------: | :-------------------------: |
|   A   |      8       |    24     |  1.0.0.0 - 126.255.255.255  |
|   B   |      16      |    16     | 128.0.0.0 - 191.255.255.255 |
|   C   |      24      |     8     | 192.0.0.0 - 223.255.255.255 |

![Network and Host Bits Image](Network-and-Host-Bits.png)

### IPv4 Address Classes(Detailed)

|     Class     |  Leading Bits  | Network Bits | Remaining Bits | Number of Networks | Hosts Per Network | Defualt Subnet Mask |
| :-----------: | :------------: | :----------: | :------------: | :----------------: | :---------------: | :-----------------: |
|       A       |   0 (1-126)    |      8       |       24       |      128(2^7)      | 16,777,216(2^24)  |      255.0.0.0      |
|       B       |  10 (128-191)  |      16      |       16       |    16,384(2^14)    |   65,536(2^16)    |     255.255.0.0     |
|       C       | 110 (192-223)  |      24      |       8        |  2,097,152(2^21)   |     256(2^8)      |    255.255.255.0    |
| D (multicast) | 1100 (224-239) | Not defined  |  Not defined   |    Not defined     |    Not defined    |     Not defined     |
| E (reserved)  | 1111 (240-255) | Not defined  |  Not defined   |    Not defined     |    Not defined    |     Not defined     |

### Defualt Subnet Masks

- The Subnet Mask tells you which portion of the IP address identifies the network and which portion identifies the host.
- Below are default Class A, B, and C Subnet Masks.

![Default-Subnet-Masks Image](Default-Subnet-Masks.png)

### CIDR Notation

- CIDR: Classless Inter-Domain Routing
  - A methodology for subnetting
  - "Slash" Notation tells you how many bits are associated with the Subnet Mask
- A shortcut way of telling us what the Subnet Mask is
  - /8 = 11111111.00000000.00000000.00000000
  - /8 = 255.0.0.0
- 192.168.1.0/24 = 255.255.255.0
- 10.1.0.0/16 = 255.255.0.0
- 196.10.10.0/25 = 255.255.255.128
