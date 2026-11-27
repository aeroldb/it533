---
layout: post
title: "Networking Fundamentals: Packet Tracer Labs 1–8"
date: 2026-11-27
categories: [Networking, Packet Tracer, Cisco]
---

# Networking Fundamentals: Packet Tracer Labs 1–8

## Introduction

This post documents my progress through eight Cisco Packet Tracer networking labs. Throughout these activities, I practiced working with Cisco IOS, configuring routers and switches, securing network devices, assigning IP addresses, connecting network equipment, and verifying network connectivity.

These exercises helped me develop practical networking skills and become more familiar with how devices communicate within a local area network (LAN) and between different networks.

---

## Lab 1: Packet Tracer – Navigate the IOS

### Objective

The objective of this lab was to become familiar with the Cisco Internetwork Operating System (IOS) command-line interface (CLI). I practiced accessing a switch through a console connection, navigating different IOS command modes, using context-sensitive help, and configuring the system clock.

### Steps

1. Connected PC1 to the S1 switch using a console cable.
2. Opened the Terminal application on PC1 to access the switch CLI.
3. Used the `?` command to display available commands and explore context-sensitive help.
4. Practiced command completion using the Tab key.
5. Entered Privileged EXEC mode using the `enable` command.
6. Entered Global Configuration mode using `configure terminal`.
7. Practiced moving between User EXEC, Privileged EXEC, and Global Configuration modes.
8. Used `show clock` to display the switch's current time.
9. Used the `clock set` command to configure the date and time.
10. Tested incomplete and invalid commands to observe how IOS displays error messages.

### Challenges

One challenge was understanding the differences between the IOS command modes and recognizing which commands were available in each mode. I also needed to become familiar with the correct syntax for configuring the system clock.

I used the question mark (`?`) and Tab completion features to identify available commands, complete command entries, and determine which parameters were required.

### What I Learned

- How to connect to a Cisco switch using a console cable.
- How to access and navigate the Cisco IOS CLI.
- The differences between User EXEC, Privileged EXEC, and Global Configuration modes.
- How to use context-sensitive help with the `?` command.
- How to use Tab completion to enter commands more efficiently.
- How to configure and verify the system clock.
- How to recognize and interpret IOS error messages.

---

## Lab 2: Packet Tracer – Basic Device Configuration

### Objective

The objective of this lab was to configure a router, a switch, and multiple end devices to establish connectivity between two LANs. I practiced basic device configuration, IPv4 and IPv6 addressing, password security, interface descriptions, and end-to-end connectivity testing.

### Steps

1. Reviewed the network topology and addressing table to identify the required IPv4 and IPv6 addresses.
2. Configured the College router with its required hostname and basic security settings.
3. Configured the Class-B switch with its hostname and device access passwords.
4. Configured the required console and privileged EXEC passwords.
5. Enabled password encryption and configured an appropriate login banner.
6. Assigned IPv4 and IPv6 addresses to the appropriate router and switch interfaces.
7. Completed the IPv4 and IPv6 addressing configurations on the PC hosts.
8. Added descriptions to network interfaces to document their connections.
9. Saved the device configurations.
10. Used ping commands to test connectivity between devices using IPv4 and IPv6.
11. Troubleshot addressing and configuration issues that could prevent end-to-end communication.

### Challenges

One of the main challenges was configuring both IPv4 and IPv6 addresses correctly across multiple devices. Each device needed the correct address, subnet information, and gateway settings.

Another challenge was ensuring that the router and switch interfaces were configured correctly and that the hosts were using the appropriate addressing information.

I approached these tasks by referring to the addressing table, checking device configurations, and using ping tests to help identify connectivity problems.

### What I Learned

- How to configure basic router and switch settings.
- How to assign IPv4 addresses to network interfaces and end devices.
- How to configure IPv6 addresses.
- The importance of default gateways for communication between networks.
- How to configure device passwords and encrypt plaintext passwords.
- How to document network interfaces using descriptions.
- How to troubleshoot network connectivity using ping.
- The importance of verifying both IPv4 and IPv6 connectivity.

---

## Lab 3: Packet Tracer – Configure Initial Switch Settings

### Objective

The objective of this lab was to learn how to perform initial configuration and security settings on Cisco switches. I practiced examining the default switch configuration, changing the hostname, securing console and privileged access, configuring an MOTD banner, and saving configuration files to NVRAM.

### Steps

1. Accessed the S1 switch through its CLI.
2. Entered Privileged EXEC mode using the `enable` command.
3. Used `show running-config` to examine the current switch configuration.
4. Reviewed the available interfaces and virtual terminal (VTY) lines.
5. Changed the switch hostname to S1.
6. Configured the console password using the `line console 0` command.
7. Enabled login authentication on the console line.
8. Configured an enable password and an encrypted enable secret.
9. Used the `service password-encryption` command to encrypt plaintext passwords.
10. Configured a Message of the Day (MOTD) banner to warn unauthorized users.
11. Verified the configuration using `show running-config`.
12. Saved the configuration using `copy running-config startup-config`.
13. Repeated the required configuration tasks on the S2 switch.

### Challenges

A challenge in this lab was understanding the difference between the enable password and the enable secret password. I also needed to understand why the `login` command was necessary when configuring console access.

Another important part was ensuring that the configuration was saved to NVRAM rather than leaving the changes only in the running configuration.

I used `show running-config` and `show startup-config` to inspect the configuration and verify the settings.

### What I Learned

- How to examine a switch's default configuration.
- How to change a switch hostname.
- How to secure console access using passwords.
- The difference between enable passwords and enable secret passwords.
- How to encrypt plaintext passwords using `service password-encryption`.
- How to configure an MOTD banner.
- The difference between running-config and startup-config.
- How to save switch configurations to NVRAM.

---

## Lab 4: Packet Tracer – Configure Initial Router Settings

### Objective

The objective of this lab was to learn how to perform initial configuration and security tasks on a Cisco router. I practiced examining the router's default configuration, securing access to the CLI and console port, configuring an MOTD banner, verifying settings, and saving the running configuration.

### Steps

1. Established a console connection between PCA and router R1.
2. Opened the Terminal application and accessed the router CLI.
3. Entered Privileged EXEC mode using the `enable` command.
4. Used `show running-config` to examine the router's current configuration.
5. Used `show startup-config` to examine the saved configuration.
6. Configured the router hostname as R1.
7. Configured the console password and privileged EXEC passwords.
8. Set an encrypted enable secret password.
9. Enabled password encryption for plaintext passwords.
10. Configured an MOTD banner displaying an unauthorized-access warning.
11. Verified the configuration using the appropriate show commands.
12. Logged out and reconnected to verify the console password and banner.
13. Saved the running configuration to NVRAM using `copy running-config startup-config`.
14. Explored the router's flash storage using `show flash`.
15. Practiced copying the startup configuration to flash as an additional backup.

### Challenges

One challenge was understanding how router access security works and how the different passwords interact. I also needed to verify that the console password, enable password, and enable secret were configured correctly.

Another challenge was understanding the difference between NVRAM and flash storage. The router uses its startup configuration from NVRAM, while flash can also store files such as the IOS image and additional configuration backups.

I used configuration display commands to inspect the settings and verify that the changes were saved.

### What I Learned

- How to establish a console connection to a Cisco router.
- How to inspect a router's running and startup configurations.
- How to configure a router hostname.
- How to secure console and privileged EXEC access.
- How to configure encrypted passwords.
- How to create an MOTD banner.
- How to save configurations to NVRAM.
- How to inspect flash storage and create an additional configuration backup.

---

## Lab 5: Packet Tracer – Basic Switch and End Device Configuration

### Objective

The objective of this lab was to configure a small LAN consisting of two Cisco switches and two end devices. I practiced assigning hostnames and IP addresses, securing switch access, encrypting passwords, configuring an MOTD banner, and verifying connectivity between the two PCs.

### Steps

1. Reviewed the addressing table to identify the required IP addresses and subnet masks.
2. Used console connections to access the ASw-1 and ASw-2 switches.
3. Configured the switch hostnames as ASw-1 and ASw-2.
4. Configured the required line passwords.
5. Configured the privileged EXEC secret password.
6. Enabled encryption for plaintext passwords.
7. Configured an appropriate MOTD banner on each switch.
8. Assigned the required management IP addresses to VLAN 1 on both switches.
9. Configured the IP addresses and subnet masks on User-01 and User-02.
10. Saved the configurations on both switches.
11. Used ping commands to verify connectivity between the two end devices.

### Challenges

One challenge was making sure that the switch management addresses and PC addresses matched the addressing table. Incorrect IP addresses or subnet masks could prevent devices from communicating.

Another challenge was applying the same security requirements consistently to both switches. I needed to verify that the hostnames, passwords, encryption settings, and banners were configured correctly.

I used the addressing table as a reference and checked the configurations before performing connectivity tests.

### What I Learned

- How to configure multiple switches using the Cisco IOS CLI.
- How to assign hostnames to network devices.
- How to configure management IP addresses on VLAN 1.
- How to assign IP addresses and subnet masks to end devices.
- How to secure switch access using passwords.
- How to configure MOTD banners and password encryption.
- How to save switch configurations.
- How to test communication between PCs on a LAN.

---

## Lab 6: Packet Tracer – Build a Switch and Router Network

### Objective

The objective of this lab was to build and configure a network consisting of a router, a switch, and two PCs. I practiced assigning static IP addresses, configuring router interfaces, verifying connectivity, examining device information, interpreting routing tables, and securing remote router access using SSH.

### Steps

1. Reviewed the network topology and addressing table.
2. Connected PC-A to S1 and connected S1 to R1 using the appropriate network cables.
3. Connected PC-B to the other router interface.
4. Configured the IP addresses, subnet masks, and default gateways on PC-A and PC-B.
5. Used ping to test connectivity between the PCs before completing the router configuration.
6. Accessed R1 through a console connection.
7. Configured the router hostname, privileged EXEC password, console password, password encryption, and MOTD banner.
8. Configured the router interfaces with the required IP addresses and enabled them using `no shutdown`.
9. Configured the switch hostname, management IP address, and default gateway.
10. Verified connectivity after completing the device configurations.
11. Used IOS show commands to examine interface statistics, interface status, and routing information.
12. Reviewed the routing table to identify directly connected networks.
13. Configured the required IP domain name and generated RSA keys.
14. Created an SSH user account.
15. Configured the VTY lines to use local authentication and allow SSH-only remote access.
16. Tested the SSH connection from a PC using the configured username and router IP address.

### Challenges

One challenge was troubleshooting connectivity before and after configuring the router interfaces. The PCs could not communicate across different networks until the router was properly configured.

Another challenge was understanding how to interpret interface status information and routing table entries. I also needed to configure SSH correctly, including the domain name, RSA keys, user credentials, and VTY line settings.

I used ping tests and IOS verification commands to check the configurations and identify areas that needed attention.

### What I Learned

- How to build a basic router-and-switch network.
- How to configure static IP addressing on PCs.
- How to configure router and switch interfaces.
- Why routers are necessary for communication between different networks.
- How to interpret routing table entries.
- How to use commands such as `show interfaces` and `show ip interface brief`.
- How to configure SSH for secure remote access.
- How to configure local user authentication on VTY lines.
- How to verify network connectivity and device configurations.

---

## Lab 7: Packet Tracer – Connect a Wired and Wireless LAN

### Objective

The objective of this lab was to practice connecting different network devices using the correct cables and ports in Cisco Packet Tracer. I also explored how wired and wireless network components connect to one another and how to examine a network using the Physical Workspace.

### Steps

1. Connected the Cloud device to Router0 using a copper straight-through cable.
2. Connected the Cloud to the Cable Modem using a coaxial cable.
3. Connected Router0 to Router1 using a serial cable.
4. Connected Router0 to the netacad.pka server using a copper crossover cable.
5. Connected Router0's console port to the Configuration Terminal using a console cable.
6. Connected Router1 to the switch using a copper straight-through cable.
7. Connected the Cable Modem to the Wireless Router's Internet port.
8. Connected the Wireless Router to the Family PC using an Ethernet cable.
9. Opened the Family PC command prompt and tested connectivity to netacad.pka using ping.
10. Opened the web browser and attempted to access `http://netacad.pka`.
11. Used the Home PC to test connectivity to the switch.
12. Accessed Router0 through the Configuration Terminal and used `show ip interface brief` to examine interface statuses.
13. Switched to the Physical Workspace and explored the Cloud, Primary Network, Secondary Network, and Home Network areas.

### Challenges

One challenge was selecting the correct cable type for each connection. Different devices and interfaces required different cables, including straight-through, crossover, coaxial, serial, and console cables.

Another challenge was understanding the difference between a console connection and a network connection. A console cable provides administrative access to a device but does not provide normal network connectivity.

I used the device interface labels and connection requirements to select the appropriate cables and checked the link indicators to help verify the connections.

### What I Learned

- How to identify the correct cable type for different network connections.
- The purpose of copper straight-through and crossover cables.
- How coaxial cables are used to connect cable modem equipment.
- How serial cables connect routers.
- How console cables provide administrative access to network devices.
- How wired and wireless network equipment can connect together.
- How to use ping and a web browser to test network connectivity.
- How to inspect router interface statuses using `show ip interface brief`.
- How to navigate the Physical Workspace in Cisco Packet Tracer.

---

## Lab 8: Packet Tracer – Connect a Router to a LAN

### Objective

The objective of this lab was to examine router information, configure router interfaces, and verify network connectivity. I practiced using Cisco IOS show commands to inspect router interfaces, understand routing table entries, configure Ethernet interfaces, and verify the network configuration.

### Steps

1. Reviewed the addressing table for R1, R2, and the four PCs.
2. Accessed the routers through their CLI interfaces.
3. Used the `show` commands to examine router interface information and the current device configuration.
4. Used `show ip route` to examine the routing table.
5. Identified directly connected networks using the routing table's connected-route entries.
6. Used interface-specific show commands to examine operational status, MAC addresses, and IP address information.
7. Used `show ip interface brief` to review interface addresses and their status.
8. Compared the router and switch interface summaries.
9. Configured the router interfaces according to the addressing table.
10. Verified the interface configurations and tested connectivity.
11. Configured the IP domain name `academy.net`.
12. Generated 1024-bit RSA keys for SSH.
13. Created a local SSH user account.
14. Configured the VTY lines to use local login authentication and permit SSH connections only.
15. Used a PC command prompt to test remote access to the router using SSH.

### Challenges

One challenge was interpreting the output from the router's show commands. The routing table, interface summaries, and detailed interface information each provide different information about the network.

Another challenge was understanding how to configure secure remote access. SSH required several configuration steps, including setting a domain name, generating RSA keys, creating a user account, and configuring the VTY lines.

I used the IOS help system and verification commands to understand the configuration requirements and inspect the router's status.

### What I Learned

- How to examine router hardware and interface information.
- How to use `show ip route` to inspect the routing table.
- How to identify directly connected networks.
- How to use `show interfaces` to examine interface details.
- How to use `show ip interface brief` to review interface status and IP addresses.
- How to configure router interfaces using IP addresses and subnet masks.
- How to verify router configurations.
- How to configure SSH using RSA keys and local user authentication.
- Why SSH is preferable to unsecured remote access methods such as Telnet.

---

## Overall Reflection

Completing these eight Packet Tracer labs helped me build a foundation in networking and Cisco device administration.

I started by learning how to navigate the Cisco IOS command-line interface. As the labs progressed, I moved on to configuring switches and routers, securing device access, assigning IPv4 and IPv6 addresses, connecting network equipment, and testing communication between devices.

One of the most important lessons from these activities was the importance of verifying configurations instead of assuming that a device is configured correctly. Commands such as `show running-config`, `show ip interface brief`, `show ip route`, and `ping` are useful tools for checking device settings and troubleshooting connectivity.

These labs also helped me understand how different networking components work together. Switches connect devices within a LAN, routers allow communication between different networks, and secure management protocols such as SSH allow administrators to remotely access network equipment.

Overall, these activities gave me practical experience with Cisco Packet Tracer and prepared me to work with more advanced networking concepts, configurations, and troubleshooting scenarios.
