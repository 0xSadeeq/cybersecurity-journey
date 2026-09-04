Network Fundamentals — Lab Summary

Objective

Investigate basic network configuration and connectivity from a Windows computer while developing an understanding of how networking concepts apply to cybersecurity.

Tools Used

- Windows Command Prompt
- "ipconfig"
- "ping"
- "nslookup"

Activities Performed

Network Configuration

Used "ipconfig" to identify the computer's:

- IPv4 address
- Subnet mask
- Default gateway

Gateway Connectivity Test

Used "ping" to verify communication between the computer and its local gateway.

Result: Successful communication was established.

Public Network Connectivity Test

Used "ping 8.8.8.8" to test connectivity to a public IP address.

Result: Successful response received.

DNS Resolution Test

Used "ping google.com" to test connectivity using a domain name.

Result: Successful response received.

DNS Investigation

Used "nslookup google.com" to observe DNS resolution.

Result: The domain was successfully resolved to an IP address and DNS server information was returned.

Security Relevance

These exercises demonstrated how basic network troubleshooting can support cybersecurity investigations.

Understanding normal network behavior provides a foundation for identifying unusual traffic, exposed services, connectivity problems, and potential attack surfaces.

Key Learning

A cybersecurity professional needs to understand how devices communicate before being able to effectively secure those communications.

This lab provided my first practical experience investigating network configuration, connectivity, and DNS resolution from the command line.
