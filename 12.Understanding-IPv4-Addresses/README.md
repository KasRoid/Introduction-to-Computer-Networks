# Understanding IPv4 Addresses

- An IP Address is a logical address used in order to uniquely identify a device on an IP network.
- It's a Network Layer address
- There are Two Versions
  - IP version 4 (IPv4)
  - IP version 6 (IPv6)

## IPv4 Address Anatomy

- Made up of 32 binary bits, which can be divided into a network portion and a host portion with the help of a subnet mask.
  - The 32 binary bits are broken into four octets (1 octet = 8 bits)
  - Each octet is converted to decimal and separated by a period (dot).
  - For this reason, an IP address is said to be expressed in dotted decimal format.

## Network and Host Portion

- An IP address is broken down into two parts
  - Network Address
    - Uniquely identifies each network
    - Your Street Name: 7682 Whilshire Drive
  - Host Address
    - Uniquely identifies each machine on a network
    - Your House Address: 7682 Wilshire Drive
- Network Address + Host Address = IP Address
  - Wilshire Drive 7682

## IPv4 Address Components

- Each device on a network is assigned an IP address, subnet mask and default gateway
  - IP Address: Unique logical address assigned to each device on a network
  - Subnet Mask: Used by the device to determine what subnet it's on, specifically the network and host portions of the IP address.
  - Default Gateway: The IP address of a network's router that allows devices on the local network to communicate with other networks.
