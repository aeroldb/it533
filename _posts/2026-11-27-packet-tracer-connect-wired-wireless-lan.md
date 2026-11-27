---
layout: post
title: "Packet Tracer – Connect a Wired and Wireless LAN"
date: 2026-11-27
categories: [Networking, Packet Tracer]
---

## Objective

The objective of this lab was to build a functional network in Cisco Packet Tracer by connecting wired and wireless network devices using the appropriate cables and interfaces.

The activity focused on understanding different cable types, establishing connections between routers, switches, computers, and wireless devices, and verifying network connectivity.

I also explored the physical topology workspace to better understand how network equipment and cabling are organized in a real-world environment.

## Steps

### 1. Connect to the Cloud

I connected Router0 to the Cloud using a Copper Straight-Through cable between Router0's FastEthernet0/0 interface and Cloud's Ethernet6 interface.

Next, I connected the Cloud's Coax7 interface to Port0 on the Cable Modem using a coaxial cable.

### 2. Connect Router0

I connected Router0 to Router1 using a serial cable, connecting Router0 Serial0/0/0 to Router1 Serial0/0.

I then connected Router0's FastEthernet0/1 interface to the netacad.pka computer's FastEthernet0 interface using a Copper Cross-Over cable.

Finally, I connected Router0's Console port to the Configuration Terminal's RS232 interface using a console cable. This allowed me to access Router0's command-line interface.

### 3. Connect the Remaining Devices

I connected Router1's FastEthernet1/0 interface to Switch FastEthernet0/1 using a Copper Straight-Through cable.

Next, I connected the Cable Modem's Port1 interface to the Wireless Router's Internet port.

I also connected the Wireless Router's Ethernet1 port to the Family PC's FastEthernet0 interface.

These connections completed the network topology.

### 4. Verify Network Connections

After completing the connections, I tested the network:

- Used the Family PC command prompt to ping netacad.pka.
- Opened the web browser and accessed http://netacad.pka.
- Used the Home PC command prompt to ping the Switch's IP address.
- Accessed Router0 through the Configuration Terminal.
- Executed `show ip interface brief` to examine interface IP addresses and operational statuses.

### 5. Examine the Physical Topology

I switched from the Logical Workspace to the Physical Workspace to explore the physical layout of the network.

I examined the Cloud, Primary Network, Secondary Network, and Home Network areas.

This allowed me to observe how network equipment, racks, and cables are organized in different environments.

## Challenges

One of the main challenges was identifying the correct cable type for each connection. Different devices and interfaces require different cables, and selecting an incorrect cable can prevent devices from communicating.

For example, connecting Router0 to the netacad.pka computer required a Copper Cross-Over cable because both devices traditionally use the same wire pairs for transmitting and receiving data.

Another challenge was understanding the difference between a console connection and a regular network connection. The console cable did not provide network connectivity, but it allowed me to access Router0's command-line interface for configuration and troubleshooting.

I addressed these challenges by reviewing device interfaces, selecting the appropriate cable types, and checking the connection indicators in Packet Tracer.

## What I Learned

This lab helped me develop a better understanding of how wired and wireless networks are physically connected.

Some of the key skills and concepts I learned include:

- **Cable selection:** Understanding when to use Copper Straight-Through, Copper Cross-Over, Serial, Coaxial, and Console cables.
- **Network interfaces:** Becoming more familiar with FastEthernet, Serial, Console, Internet, and Ethernet interfaces.
- **Router connectivity:** Understanding how routers connect different networks and communicate with other networking devices.
- **Wireless networking:** Learning how a wireless router connects to a cable modem and provides network access to connected devices.
- **Network troubleshooting:** Using ping commands and `show ip interface brief` to verify connectivity and inspect interface statuses.
- **Physical topology:** Understanding how network equipment and cabling are arranged in physical environments.

Overall, this activity strengthened my understanding of basic network infrastructure and the importance of selecting the correct cables, connecting devices properly, and verifying network connectivity.

## Lab Results

_Add screenshots of your completed Packet Tracer topology, successful ping tests, and Router0 interface status here._
