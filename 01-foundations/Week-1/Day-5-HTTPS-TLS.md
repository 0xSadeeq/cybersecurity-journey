Week 1 — Day 5: HTTPS, TLS & Secure Web Traffic

Objective

Learn the basic difference between HTTP and HTTPS, understand the role of TLS, and use Termux to inspect a website's TLS connection.

 What I Learned

HTTP

HTTP (Hypertext Transfer Protocol) is used for communication between a client and a web server.

- Commonly uses port 80
- Does not provide TLS encryption

HTTPS

HTTPS (HTTP Secure) is HTTP protected by TLS.

- Commonly uses port 443
- Provides encrypted communication
- Uses digital certificates to help verify the server's identity

TLS

TLS (Transport Layer Security) provides security for HTTPS connections.

It helps provide:

- Encryption
- Authentication
- Integrity protection

Practical Work

I used Termux and OpenSSL to inspect TLS connections.

1. Checked OpenSSL

openssl version

2. Inspected Google's TLS connection

openssl s_client -connect google.com:443 -servername google.com

The TLS connection returned a certificate and showed:

Verify return code: 0 (ok)

3. Inspected GitHub's TLS connection

openssl s_client -connect github.com:443 -servername github.com

The certificate verification succeeded.

4. Tested TLS on port 80

openssl s_client -connect github.com:80 -servername github.com

The connection did not provide a peer certificate because port 80 normally serves HTTP rather than HTTPS/TLS.

5. Compared HTTP and HTTPS

curl -I http://github.com

curl -I https://github.com

I used the commands to compare the HTTP and HTTPS responses.

Key Lesson

HTTP and HTTPS are not the same.

HTTPS uses TLS to protect web communication.

A simple way to remember:

HTTP → Port 80

HTTPS → Port 443 → TLS → Secure communication

Tools Used

- Termux
- OpenSSL
- cURL
- GitHub

 Reflection

Today I learned how HTTPS protects web traffic and how TLS certificates are involved in establishing a secure connection. I also used command-line tools to inspect real TLS connections instead of only learning the concepts theoretically.

Practical Evidence

Google TLS Connection

"Google TLS connection" (./google-tls.png)

GitHub TLS Connection

"GitHub TLS connection" (./github-tls.png)
