# Wireless Networking and IoT

## Overview of Wireless Networking

- IEEE 802.11: Standard for Wireless Networking
  - Been updated over the last 20 years with numerous improved 802.11 standards:
    - 802.11a
    - 802.11b
    - 802.11g
    - 802.11n
    - 802.11ac
- Wireless LANs (WLANs) use radio frequencies (RFs) that are radiated into the air from an antenna that creates radio waves.
- Can extend the connection of a wired network, used to connect entire local area networks or connect different networks together.

### Depicting Wireless Networks

![Depicting-Wireless-Networks Image](Depicting-Wireless-Networks.png)

### Wireless Access Point (WAP)

- A Wireless Access Point (WAP) is a bridge that extends the wired network to the wireless network.
- Just like a switch and a wired bridge, it's a Data Link Layer 2 device.
- Note: A WAP is not a router.

![Wireless Access Point Image](Wireless-Access-Point.png)

### Antennas

![Antennas Image](Antennas.png)

- Antenna strength measured in dBi. The higher the dBi, the further distance the signal will travel.

### Service Set Identifier (SSID)

- All wireless networks have a Service Set Identifier (SSID) in infrastructure mode.
- The SSID is the wireless network's name.
- Wireless access points broadcast a wireless network's SSID. so it is viewable by devices with a wireless network adapter.
- For network security reasons, SSID broadcasting can be disabled.

![Service Set Identifier Image](Service-Set-Identifier.png)

### CSMA/CA

- CSMA/CA: Carrier Sense Multiple Access with Collision Avoidance
- While wired Ethernet networks use CSMA/CD, wireless Ethernet networks use CSMA/CA.
- With wireless networks, it's more difficult to detect collisions, so CSMA/CA tries to avoid them with RTS and CTS:
  - Request to Send (RTS)
  - Clear to Send (CTS)

![CSMA/CA Image](CSMA-CA.png)

---

## Understanding Service Set Types

### Service Set Types

- There are three service types:
  - Independent Basic Service Set (IBSS)
  - Basic Service Set (BSS)
  - Extended Service Set (ESS)

### Ad hoc Mode: Independent Basic Service Set (IBSS)

- Peer-to-peer (P2P) wireless network shere no wireless access point (WAP) infrastructure exists.
- The devices communicate directly with one another.
- Personal area networks (PANs) are a common example of Ad hoc wireless networks.

### infrastructure Mode

Basic Service Set (BSS)

- Single Wireless Access Point (WAP)
- Most common configuration

![Basic Service Set Image](Basic-Service-Set.png)

Extended Service Set (ESS)

- Multiple WAPs, utilizing the same SSID
- Allows wireless users to seamlessly "roam" from one WAP to another.

![Extended Service Set Image](Extended-Service-Set.png)

---

## Wireless Frequencies and Channels

### Understanding Wireless Frequencies

- Wireless signals occuoy a spectrum of frequencies:
  - Signals that vibrate slowly have a low frequency.
  - Signals that vibrate quickly have a high frequency.
- For example:
  - AM Radio: 10MHz
  - FM Radio: 100MHz
  - Microwave Oven: 2.4GHz
  - Cordless Phone: 2.4GHz
- 802.11 Wireless operates at either 2.4Ghz or 5GHz

### Understanding Wireless Channels

- 802.11 Wi-Fi communication also operates on a channel, which is a portion of the 2.4GHz or 5GHz spectrum.
- 2.4GHz Band
  - Compsed of 14 overlapping 20MHz channels. Due to licensing laws:
    - Only channels 1 through 11 available in the United States.
    - Most other countries allow channels 12 and 13.
    - Channel 14 is only available in Japan.
  - It's recommended to use channels 1, 6 or 11 because they do not overlap.
    - There are just 3 non-overlapping channels.
    - ![2.4GHz Band Image](2.4GHz-Band.png)
- 5GHz Band
  - 5GHz offers significantly more channels than 2.4GHz.
  - There are roughly 40 different non-overlapping 20MHz channels.
  - Different countries have widely different rules for which channels can be used.
    - 24 non-overlapping channels available in North America.
    - 802.11 features 5GHz auto-channel switching.

### Understanding Channel Bandwidth

- The width of a channel is a channel's Bandwidth
- Expressed in MHz but equates to how many vits can be transmitted per second.
- The larger the channel bandwidth, the faster the data throughput.
- In 802.11, channel bandwidth varies from 20MHz up to 160MHz

### Understanding Channel Bonding

- 802.11 provides a channel bonding feature:
  - When two adfacent channels are combined (bonded together) to increase bandwidth.
  - When channels are bonded together, their bandwidths doubles.
  - 20MH channels can be bonded to 40MHz, 80MHz, or 160MHz Channels

![Channel Bonding Image](Channel-Bonding.png)

### 2.4GHz versus 5GHz

- 2.4GHz Frequency Band
  - Longer Frequency Waves
    - Prorogates through solid surfaces well
    - Good solution for long-distances
    - Slower data rates
  - Lower data rates over longer distances
  - Fewer Channels
    - 3 non-overlapping channels
  - Suffers from frequency congestion & interference
    - Microwaves, cordless phones, and Bluetooth operate at 2.4GHz
- 5GHz Frequency Band
  - Shorter Frequency Waves
    - Less effective penetrating solid surfaces
    - Not as effective over long-distances
    - Faster data rates
  - Higher data rates over shorter distances
  - More Channels
    - 24 non-overlapping channels
    - Channel bonding available
  - Less congested than 2.4 GHz frequency
    - Frequency congestion and interference isn't a big issue.
