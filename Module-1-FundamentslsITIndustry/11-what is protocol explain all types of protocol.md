# What Is a Network Protocol?

A **network protocol** is an agreed set of rules that devices and software use to communicate. Protocols define how information is formatted, addressed, transmitted, received, and sometimes checked for errors or protected.

For example, when you open a website, your device may use DNS to look up its domain name, IP to address network traffic, TCP or QUIC to transport data, and HTTP or HTTPS to request the page.

There are many protocols, and new ones continue to be developed. They are often grouped by the communication task or network layer they support.

## Common Protocol Groups and Examples

### 1. Application-Layer Protocols

Application-layer protocols define communication for services people and programs use, such as websites, email, and file transfer.

- **HTTP (Hypertext Transfer Protocol):** Transfers web requests and responses.
- **HTTPS (HTTP Secure):** HTTP communication protected with TLS encryption and authentication.
- **DNS (Domain Name System):** Looks up information such as the IP address associated with a domain name.
- **SMTP (Simple Mail Transfer Protocol):** Sends email between mail clients and servers or between mail servers.
- **IMAP (Internet Message Access Protocol):** Lets an email client access and manage messages stored on a mail server.
- **POP3 (Post Office Protocol version 3):** Lets an email client retrieve messages from a mail server, commonly by downloading them.
- **FTP (File Transfer Protocol):** Transfers files, but basic FTP does not encrypt the connection.
- **SFTP (SSH File Transfer Protocol):** Transfers and manages files over an SSH-secured connection. Despite the name, it is not simply FTP with encryption.
- **SSH (Secure Shell):** Provides secure remote login and command execution.
- **DHCP (Dynamic Host Configuration Protocol):** Automatically provides network configuration, such as an IP address, to devices.
- **NTP (Network Time Protocol):** Synchronizes clocks on computers over a network.
- **SNMP (Simple Network Management Protocol):** Helps monitor and manage network devices.

### 2. Transport-Layer Protocols

Transport protocols carry data between applications running on networked devices. They use port numbers to direct traffic to the right application.

- **TCP (Transmission Control Protocol):** Establishes a connection and provides reliable, ordered delivery. It retransmits data when needed. Web, email, and file-transfer services commonly use TCP.
- **UDP (User Datagram Protocol):** Sends independent datagrams without establishing a connection or guaranteeing delivery and order. It has less built-in overhead and is useful for applications such as real-time audio, video, and some games.
- **QUIC:** A modern transport protocol built on UDP that provides features such as secure connections and reliable streams. HTTP/3 uses QUIC.

The best transport depends on the needs of the application. UDP is not automatically faster or better; the application may need to handle delivery and ordering itself.

### 3. Internet or Network-Layer Protocols

These protocols help identify devices and move packets between networks.

- **IP (Internet Protocol):** Provides addressing and routing for packets. Its main versions are **IPv4** and **IPv6**.
- **ICMP (Internet Control Message Protocol):** Carries network status and error information. Tools such as `ping` commonly use ICMP messages.
- **IPsec (Internet Protocol Security):** A set of protocols used to protect IP traffic, often in virtual private networks (VPNs).

### 4. Link and Local-Network Protocols

Link-layer protocols carry data across a local network connection.

- **Ethernet:** Commonly connects devices on wired local area networks (LANs).
- **Wi-Fi (IEEE 802.11):** Connects devices to local networks wirelessly.
- **ARP (Address Resolution Protocol):** In IPv4 local networks, helps find the link-layer address associated with a local IP address. IPv6 uses Neighbor Discovery instead.
- **PPP (Point-to-Point Protocol):** Carries network traffic over a direct point-to-point link; it is used in some access technologies.

### 5. Routing Protocols

Routing protocols help routers exchange information and choose paths for traffic between networks.

- **BGP (Border Gateway Protocol):** Exchanges routing information between large independently managed networks on the internet.
- **OSPF (Open Shortest Path First):** Finds routes within an organization's or provider's network.
- **RIP (Routing Information Protocol):** A simpler routing protocol historically used in smaller networks; it is less common in modern large networks.

### 6. Security Protocols

Security protocols protect communication, help authenticate parties, or establish secure connections.

- **TLS (Transport Layer Security):** Protects data in transit and helps authenticate a server. HTTPS uses TLS.
- **SSH:** Protects remote sessions and can also provide secure tunneling and file transfer.
- **IPsec:** Protects IP traffic at the network layer.
- **WPA2 and WPA3:** Security standards used to protect access to Wi-Fi networks.

Security depends on correct configuration, up-to-date software, and trustworthy endpoints; using a security protocol alone does not guarantee that an entire system is safe.

## Protocols Work Together in Layers

Communication usually uses several protocols together rather than just one. For example, loading an HTTPS website may involve:

1. **Wi-Fi or Ethernet** to send data across the local connection.
2. **IP** to route packets between networks.
3. **TCP** or **QUIC** to transport application data.
4. **TLS** to protect the connection (with QUIC integrating security).
5. **HTTP** to request and deliver web resources.
6. **DNS** to look up a domain name when its address is needed.

The exact combination varies. For instance, HTTP/3 uses QUIC rather than TCP.

## Protocol vs. Protocol Suite

A **protocol** is a set of communication rules. A **protocol suite** is a collection of related protocols designed to work together. The **TCP/IP suite** is the foundation of communication on the internet and includes protocols such as IP, TCP, UDP, and application-layer protocols.

## Why Protocols Matter

Protocols allow devices and software made by different organizations to communicate consistently. They support:

- Interoperability between different systems
- Addressing and routing data
- Reliable or real-time delivery, depending on the need
- Common services such as web browsing, email, and file transfer
- Security and network management

## Conclusion

A network protocol is a shared set of rules for communication. Protocols are commonly grouped by layer: application protocols provide services such as web and email; transport protocols carry application data; internet-layer protocols address and route packets; and link-layer protocols move data across local connections. Multiple protocols work together whenever devices communicate.