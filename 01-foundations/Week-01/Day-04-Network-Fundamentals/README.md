Week 1 — Day 4: Network Security Fundamentals

Objective

Learn the fundamentals of computer networking and understand how networking concepts relate to cybersecurity and network security.

 Topics Covered

- Computer networks
- LAN and WAN
- IP addresses
- Routers and switches
- Subnet masks
- Default gateways
- Firewalls
- Ports and protocols
- DNS
- Network segmentation
- Attack surface

 Key Concepts Learned

Computer Network

A computer network is a group of devices that communicate with each other and share resources.

Router vs Switch

- Router: Connects and moves traffic between different networks.
- Switch: Connects devices within a local network.

IP Address

An IP address identifies a device/interface on a network and allows network traffic to be addressed to it.

Subnet Mask

A subnet mask helps determine which part of an IP address represents the network and which part identifies the host.

Default Gateway

The default gateway is usually the router that a device uses to communicate with destinations outside its local network.

Firewall

A firewall controls network traffic according to configured security rules. It can allow or block traffic based on factors such as source, destination, protocol, and port.

Ports and Services

A port can be thought of as a specific communication endpoint for a service.

Examples:

- 22 — SSH
- 53 — DNS
- 80 — HTTP
- 443 — HTTPS
- 23 — Telnet

Unnecessary exposed services can increase an organization's attack surface.

DNS

DNS (Domain Name System) translates human-readable domain names into IP addresses.

Example:

"google.com → DNS → IP address"

🛡️ Network Segmentation

Network segmentation separates devices and systems into different network segments.

For example:

"Employee Network → Internal Systems"

"Guest Network → Internet"

Proper segmentation can limit an attacker's ability to move from a compromised device into sensitive internal systems.

This introduced me to the concept of lateral movement, where an attacker attempts to move from one compromised system to other systems within a network.

Hands-On Practice

1. Network Configuration

Used:

"ipconfig"

to inspect my computer's network configuration.

I identified:

- IPv4 address
- Subnet mask
- Default gateway

2. Gateway Connectivity

Used:

"ping <default-gateway>"

to test communication between my computer and the local gateway.

3. Internet Connectivity

Used:

"ping 8.8.8.8"

to test connectivity to a public IP address.

4. DNS Connectivity

Used:

"ping google.com"

to test connectivity using a domain name.

5. DNS Lookup

Used:

"nslookup google.com"

to observe how DNS resolves a domain name to an IP address.

Security Takeaways

Today I learned that network security involves understanding how devices communicate before trying to secure them.

Important questions a security professional should ask include:

- What devices are communicating?
- What network are they on?
- What services are exposed?
- Which ports are open?
- Is the traffic legitimate?
- Can a firewall restrict the traffic?
- Is the network properly segmented?
- Could an attacker move laterally after compromising a device?

What I Learned Today

I moved from basic cybersecurity concepts into practical network investigation using the Windows command line.

Tools/commands practiced:

- "ipconfig"
- "ping"
- "nslookup"

This is the beginning of my hands-on Network Security learning path.
