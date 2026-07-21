Assignment
Title

How the Internet Delivers a Web Page — A Case Study on Instagram

Objective

To understand and explain the complete process that occurs when a user types a website URL (https://www.instagram.com) into a web browser and presses Enter — covering the TCP/IP protocol stack, DNS resolution, HTTP communication, TCP reliability, client-server architecture, and the role of cookies — in order to appreciate how application-layer protocols work together to deliver a seamless Internet experience.

Solution

1. TCP/IP Protocol Stack
The TCP/IP model has five layers, each with a distinct role:

Application Layer – generates the HTTP/HTTPS request (protocols: HTTP, HTTPS, DNS, FTP, SMTP, POP3, IMAP, DHCP)
Transport Layer – provides reliable (TCP) or fast/connectionless (UDP) end-to-end delivery
Network Layer – handles logical addressing and routing (IP, ICMP, ARP)
Data Link Layer – handles node-to-node delivery on the local network (Ethernet, Wi-Fi, MAC)
Physical Layer – transmits raw bits as electrical, optical, or radio signals

2. DNS Resolution
When the user types www.instagram.com, the browser and OS check their cache, and if not found, the request goes to a DNS resolver/server, which returns the IP address (e.g., 157.240.x.x) so the browser can locate the server.

3. HTTP Request/Response
After obtaining the IP address, the browser opens a connection and sends an HTTP GET request (GET / HTTP/1.1, Host: www.instagram.com). The server processes it and returns HTML, CSS, JavaScript, images, and videos, which the browser renders.

4. TCP Reliability
Before data transfer, TCP performs a three-way handshake (SYN → SYN-ACK → ACK) to establish a connection. TCP then guarantees reliable, ordered, error-checked delivery through retransmission, flow control, and congestion control.

5. Client–Server Architecture
Instagram follows a Client–Server model: the browser (client) sends requests, and Instagram's servers process them and respond — there is no direct peer-to-peer exchange between users' devices.

6. HTTP vs FTP

HTTP:                         
 Accesses web pages	          
 Port 80/443	
 Stateless
 Used by browsers
 FTP:
  Transfers files
  Port 21
 	Session-oriented
  Used by FTP clients


7. Role of Cookies
Cookies are small files stored by the browser that let Instagram remember login sessions, preferences (e.g., dark mode), and browsing activity — enabling personalized feeds and recommendations without repeated logins.

Output
>The browser successfully resolves www.instagram.com to its IP address via DNS.
>A TCP connection is established using the three-way handshake.
>The HTTP GET request retrieves the Instagram homepage content (HTML, CSS, JS, media).
>The browser renders and displays the personalized Instagram feed to the user, with login state and preferences preserved via cookies.

Conclusion
Application-layer protocols play a vital role in everyday Internet communication by enabling users to access websites, send emails, transfer files, and use online services efficiently. Protocols such as HTTP/HTTPS, DNS, FTP, and SMTP ensure smooth and secure communication between users and servers. In the case of Instagram, DNS converts the domain name into an IP address, HTTP/HTTPS securely delivers the webpage along with images and videos, and cookies improve the browsing experience by remembering user preferences and login details. Together with the TCP/IP model, these protocols provide reliable, fast, and secure data transmission — making Internet services simple, efficient, and user-friendly.
