# Chapter 6: Networks, Internet & Security

## Overview

- Network classifications, devices, and topologies.
- Internet fundamentals: TCP/IP, DNS, and the Web.
- Security: privacy, authentication, and trust.

## Module 01: Network Fundamentals

### What is a Network?

A network consists of connected devices that share data and resources.

- **Links** may be wired, wireless, or both.
- **Protocols** define the rules of communication.

### Network Classifications

| Type | Definition | Example |
|---|---|---|
| **PAN** | Personal Area Network: Devices near one person. | Bluetooth earbuds. |
| **LAN** | Local Area Network: Devices in a home, school, or office. | Home Wi-Fi network. |
| **MAN** | Metropolitan Area Network: Connections across a city or large urban area. | City-wide broadband. |
| **WAN** | Wide Area Network: Links across countries or long distances. | The Internet. |

### Network Building Blocks

A functioning network needs nodes, links, and rules.

- **Endpoints:** Computers, phones, printers, and servers that send or receive data.
- **Media:** Ethernet cables, fiber optics, and radio waves that carry signals.
- **Devices:** Switches, routers, and access points that connect network segments.

### Know Your Devices

- **Modem:** Provides access to a service-provider link in many setups.
- **Switch:** Connects devices within a local network and forwards frames.
- **Router:** Forwards packets between IP networks, often connecting a LAN to the Internet.
- **Access Point:** Connects wireless clients to a network using Wi-Fi.

### Network Topologies

Topology describes how devices and links are arranged.

| Topology | Description | Pros / Cons |
|---|---|---|
| **Star** | Devices link to a central switch or hub. | Easy to manage; central point matters. |
| **Mesh** | Nodes use multiple links. | Offers alternate paths but can be complex. |
| **Bus** | Devices share a common line. | Simple design; failures and contention matter. |

## Module 02: Internet Fundamentals

### Internet vs. World Wide Web

- **Internet:** A global system of interconnected networks. It carries many services (e.g., email, online games).
- **Web:** A service on the Internet consisting of linked pages and resources accessed by browsers (e.g., websites).

### The TCP/IP Model

Each layer has a different responsibility.

1. **Application:** Protocols for services such as HTTP, DNS, and email.
2. **Transport:** TCP provides reliable streams; UDP sends datagrams.
3. **Internet:** IP addresses packets and supports routing between networks.
4. **Link:** Ethernet and Wi-Fi move data over the local link.

### IP, Packets & Routers

- **IP Address:** A logical address that helps identify where an IP packet should go.
- **Packets:** Data is split and carried in packets with routing information. They can take different paths through the network.
- **Routers:** Forward packets toward destinations across networks.

### How DNS Works

DNS translates human-readable names into address records.

1. **Enter name:** You type a domain such as `example.com`.
2. **Look up:** A DNS resolver finds the relevant address record.
3. **Get address:** The resolver returns an IP address to the client.
4. **Connect:** The browser can connect to the destination service.

### A Web Request

1. **Browser:** Identifies the requested resource.
2. **DNS:** Obtains an IP address for the host.
3. **HTTPS:** Makes a secure web request using supported protocols.
4. **Response:** The server sends content for the browser to display.

## Module 03: Security Essentials

### Four Security Goals

1. **Privacy:** Limit inappropriate exposure or use of personal information.
2. **Authentication:** Verify the identity of a user, device, or service.
3. **Integrity:** Detect unauthorized changes to data or messages.
4. **Nonrepudiation:** Provide credible evidence of who approved or sent an action.

### Tools for Digital Trust

- **Encryption:** Protects data from unauthorized reading (e.g., during an HTTPS connection).
- **MFA (Multi-Factor Authentication):** Adds a second verification factor beyond a password.
- **Digital Signatures:** Can verify a signer and detect tampering; trusted keys matter.

### Threats and Defenses

| Threat | Description | Defense |
|---|---|---|
| **Phishing** | Fake messages steal credentials. | Verify senders and links. |
| **Malware** | Malicious code disrupts systems. | Update software and use backups. |
| **Interception** | Attackers may observe network traffic. | Use HTTPS and secured Wi-Fi. |

### One Secure Transaction

- **Privacy:** Encrypt sensitive information in transit.
- **Authentication:** Verify the account with MFA.
- **Integrity and proof:** Use trusted records or signatures.

## Key Takeaways

- Networks connect devices using shared rules.
- TCP/IP, IP addresses, and DNS power Internet use.
- Security protects privacy, identity, and data integrity.
