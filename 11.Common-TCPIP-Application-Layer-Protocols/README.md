# Coomon TCP/IP Application Layer Protocols

## Application Layer Management Protocols

- Domain Name System (DNS)
- Dynamic Host Configuration Protocol (DHCP)
- Network Time Protocol (NTP)
- Simple Network Management Protocol (SNMP)
- Lightweight Directory Access Protocol (LDAP)
- LDAP Secure (LDAPS)
- Server Message Block (SMB)

### Domain Name System (DNS)

- Port: 53, Transport Layer Protocol: UDP
- Protocol that is used to resolve a domain name to its corresponding IP address
  - InstructorAlton.com -> 162.0.232.236
- Uses TCP port 53 by default
- We'll be discussing DNS in detail in the DNS Network Services section of this course
  - DNS Hierarchy
  - DNS Record Types
  - Name Resolution

### Dynamic Host Configuration Protocol (DHCP)

- Port: 67, 68, Transport Layer Protocol: UDP
- Protocol that automatically assigns IP address configuration to devices on a network
  - IP address
  - Subnet Mask
  - Default Gateway
  - DNS Server

### Network Time Protocol (NTP)

- Port: 123, Transport Layer Protocol: TCP
- Protocol that automatically synchronizes a system's time with a network time server.
  - Important for time-dependent network applications and protocols.
  - If a system is configured with the incorrect time, it may not be able to access network services.
  - Authentication will often fail if time isn't properly synchronized between devices.

### Simple Network Management Protocol (SNMP)

- Port: 161, Transport Layer Protocol: TCP
- Protocol used to monitor and manage network devices.
- Allows admins to monitor and manage network devices and traffic.
- Allows network devices to communicate information about their state
  - Memory
  - CPU
  - Bandwidth

### Lightweight Directory Access Protocol (LDAP)

- Port: 389, Transport Layer Protocol: TCP
- Protocol that provides a means to access and query directory service systems
  - Usernames, Passwords, Computer Accounts, etc.
- Typically Unix/Linux-based or Microsoft Active Directory-based

### LDAP Secure (LDAPS)

- Port: 636, Transport Layer Protocol: TCP
- LDAP over SSL
- A secure versio of LDAP that utilizes SSL to encrypt LDAP network traffic.

### Server Message Block (SMB)

- Port: 445, Transport Layer Protocol: TCP
- Networkk and file sharing protocol commonly used in Microsoft environments
- Allows systems to share their files and printers with other systems
