# My Home Network Documentation
## 1. Introduction
This document provides a detailed overview of the physical and logical topologies of the home network. It includes addressing schemes, device information, network configurations, and details about the security of login credentials. The aim is to offer a clear map of the network for troubleshooting, maintenance, and security purposes.
## 2. Physical and Logical Topologies
### 2.1 Physical Topology
The physical topology refers to the physical arrangement of devices and cables that interconnect them. The home network uses a star topology, where all devices connect to a central router.
#### Devices Connected:
* Router (Primary Network Hub): Connected to the modem, distributing network connectivity.
* Switch (If applicable): Used to extend the number of wired connections in certain rooms.
* Devices: Include laptops, smartphones, smart TVs, printers, and desktop computers.

#### Physical Layout:
* Router: Positioned in a central location, connecting to the modem and all other devices.
* Wired Devices: Desktop computers and media devices connected to the router and switch via Ethernet cables.
* Wireless Devices: Laptops, smartphones, smart TVs, and IoT devices connected to the router via Wi-Fi.

### 2.2 Logical Topology
The logical topology refers to the logical connections between devices, such as IP addressing and routing.
* Router: Manages DHCP and handles IP address assignments for the home network.
* LAN (Local Area Network): All devices are connected within a single subnet.
* WIFI Networks: Two separate networks, one for personal use and one for IoT devices (isolated for security).
* Subnet Mask: 255.255.255.0 (standard for home networks, providing up to 254 devices).
#### Network Segmentation:
* Main Network: Devices like computers, printers, and smartphones.
* Guest Network: Devices for guests to access the internet, but isolated from the main network.
* IoT Network: Devices like smart thermostats, cameras, and light bulbs, isolated for security purposes.
### 3. Addressing Documentation
#### IP Addressing Scheme:
The home network uses private IP address ranges as defined by RFC 1918 for local communication. The router’s IP is set as the gateway.
Device  |	IP Address  |	Subnet Mask  |	Purpose  |
--------|-------------|--------------|-----------|
Router  |192.168.x.x  |255.255.255.0 |Default Gateway
Desktop (Wired) | 192.168.x.x | 255.255.255.0 | Home Workstation use
Laptop (Wi-fi) | 192.168.x.x | 255.255.255.0 | Personal Laptop
Smartphone | 192.168.x.x | 255.255.255.0 | Personal Phone 
Smart TV | 192.168.x.x | 255.255.255.0 | Entertainment
Printer | 192.168.x.x | 255.255.255.0 | Office Printer
Camera | 192.168.x.x | 255.255.255.0 | CCTV
### 4. Device Information
 #### Router:
    Model: ASUS RT-AC68U
    IP Address: 192.168.x.1
    Features: Dual-band Wi-Fi (2.4 GHz, 5 GHz), supports VLANs for network segmentation, QoS for prioritizing traffic, built-in firewall.
  #### Desktop:
    Model: Dell XPS 15
    OS: Windows 11
    Connection: Wired Ethernet via Router
  #### Laptop:
    Model: Apple MacBook Air
    OS: macOS
    Connection: Wi-Fi (Connected to 2.4 GHz network)
  #### Smartphone:
    Model: Samsung Galaxy S21
    OS: Android
    Connection: Wi-Fi (Connected to 5 GHz network)
  #### Smart TV:
    Model: Samsung 4K UHD TV
    Connection: Wired Ethernet (via switch)
  #### Printer:
    Model: HP LaserJet Pro MFP
    Connection: Wired Ethernet (Static IP 192.168.x.x)
  #### Cameras:
    Models: Ring Indoor Cameras
    Connection: Wi-Fi (on IoT VLAN)
### 5. Maintain Configurations
All configuration changes and device settings are maintained by a network administrator, who ensures that:
* **Router Configuration:** Regularly backed up to an external storage device.
* **Firmware:** Router and device firmware are updated regularly for security patches.
* **VLAN Settings:** IoT devices are on a separate VLAN to minimize security risks.
* **Wi-Fi Settings:** WPA3 encryption is used for Wi-Fi security, and the password is changed every 3 months.
* **Device Configurations:** Static IPs and reserved DHCP ranges are documented to avoid IP conflicts.
### 6. Network topology Diagram


### 7. Conclusion
This documentation provides a clear overview of the physical and logical network setup, device details, IP addressing scheme, and security protocols used within the home network. By maintaining these configurations and securely storing credentials, we ensure the network is reliable, secure, and scalable for future growth.







