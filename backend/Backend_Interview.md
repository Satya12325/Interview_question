# What is Caching? How can you save money with Caching?

Ans-Caching is the process of storing copies of files in a cache, or temporary storage location,
so that they can be accessed more quickly. Technically, a cache is any temporary storage location
for copies of files or data, but the term is often used in reference to Internet technologies.
Web browsers cache HTML files, JavaScript, and images in order to load websites more quickly,
while DNS servers cache DNS records for faster lookups and CDN servers cache content to reduce latency.

# What is Strong Consistency?

Strong consistency is one of the consistency models used in the domain of concurrent programming (e.g., in distributed shared memory, distributed transactions).

The protocol is said to support strong consistency if:

All accesses are seen by all parallel processes (or nodes, processors, etc.) in the same order (sequentially)
Therefore, only one consistent state can be observed, as opposed to weak consistency, where different parallel processes (or nodes, etc.) can perceive variables in different states.



# Q.What is load balancing?

Load balancing refers to efficiently distributing incoming network traffic across a group of backend servers,
also known as a server farm or server pool.
Modern high‑traffic websites must serve hundreds of thousands, if not millions, of concurrent
requests from users or clients and return the correct text, images, video, or application data, all in a fast and
reliable manner. To cost‑effectively scale to meet these high volumes, modern computing best practice generally requires
adding more servers.

# Q.What is CAP Theorem?

Ans-The CAP theorem, originally introduced as the CAP principle, can be used to explain some of the
competing requirements in a distributed system with replication. It is a tool used to make system designers
aware of the trade-offs while designing networked shared-data systems.
The three letters in CAP refer to three desirable properties of distributed systems with replicated data:
consistency (among replicated copies), availability of the system for read and write operations) and
partition tolerance in the face of the nodes in the system being p

# Q.What is PACELC Theorem?

Ans-The PACELC theorem is an extension to the CAP theorem.
Both theorems were developed to provide a framework for comparing distributed systems.
Like the CAP theorem, the PACELC theorem states that in case of network partitioning (P)
in a distributed computer system, one has to choose between availability (A) and consistency (C).
PACELC extends the CAP theorem by introducing latency and consistency as additional attributes of
distributed systems. The theorem states that, "else (E), even when the system is running normally
in the absence of partitions, one has to choose between latency (L) and consistency (C)."

# Q.What are message queues?

ans-A message queue provides an asynchronous communications protocol, which is a system that puts
a message onto a message queue and does not require an immediate response to continuing processing.
Email is probably the best example of asynchronous communication. When an email is sent, the sender
continues to process other things without needing an immediate response from the receiver. This way of
handling messages decouples the producer from the consumer so that they do not need to interact with
the message queue at the same time.

# Q-What are the different types of databases?

ans-

Depending upon the usage requirements, there are following types of databases available in the market −

* Centralised database.
* Distributed database.
* Personal database.
* End-user database.
* Commercial database.
* NoSQL database.
* Operational database.
* Relational database.
* Cloud database.
* Object-oriented database.
* Graph database.

<img src="https://www.tutorialspoint.com/assets/questions/images/113180-1532341943.jpg" />

# Q.What are webhooks?

ans-Webhooks are one way that apps can send automated messages or information to other apps. It's how PayPal tells your accounting app when your clients pay you, how Twilio routes phone calls to your number, and how WooCommerce can notify you about new orders in Slack.

# What is Docker? Why do we use it?

Docker, a subset of the Moby project, is a software framework for building, running, and managing
containers on servers and the cloud. The term "docker" may refer to either the tools
(the commands and a daemon) or to the Dockerfile file format.

It used to be that when you wanted to run a web application, you bought a server, installed Linux, set up a LAMP stack, and ran the app. If your app got popular, you practiced good load balancing by setting up a second server to ensure the application wouldn't crash from too much traffic.

# What is Cloudfront in AWS?

Amazon CloudFront is a web service that speeds up distribution of your static and dynamic web content,
such as . html, . css, . js, and image files, to your users. CloudFront delivers your content through
a worldwide network of data centers called edge locations.

# Q.What is Route 53 In AWS?

Amazon Route 53 is a highly available and scalable Domain Name System (DNS) web service. It is designed
for developers and corporates to route the end users to Internet applications by translating human readable
names like www.mydomain.com, into the numeric IP addresses like 192.0.2.1 that computers use to connect to each other.

# Q.What are ELBs in AWS?

Ans-AWS Elastic Load Balancer (ELB) automatically distributes your incoming traffic across multiple targets,
such as EC2 instances, containers, and IP addresses, in one or more Availability Zones. It monitors the health
of its registered targets, and routes traffic only to the healthy targets. Elastic Load Balancing scales your load balancer as your incoming traffic changes over time. It can automatically scale to the vast majority of workloads.

# What is TLS?

Ans-TLS is a cryptographic protocol that provides end-to-end security of data sent between applications over the Internet. It is mostly familiar to users through its use in secure web browsing, and in particular the padlock icon that appears in web browsers when a secure session is established. However, it can and indeed should also be used for other applications such as e-mail, file transfers, video/audioconferencing, instant messaging and voice-over-IP, as well as Internet services such as DNS and NTP.

# What is the difference HTTPS vs HTTP?

ans-In HTTP, URL begins with "http://" whereas URL starts with "https://"
HTTP uses port number 80 for communication and HTTPS uses 443
HTTP is considered to be unsecure and HTTPS is secure
HTTP Works at Application Layer and HTTPS works at Transport Layer
In HTTP, Encryption is absent and Encryption is present in HTTPS as discussed above
HTTP does not require any certificates and HTTPS needs SSL Certificates

# What is a reverse proxy?

A reverse proxy is a server that sits in front of web servers and forwards client (e.g. web browser) requests to those web servers. Reverse proxies are typically implemented to help increase security, performance, and reliability.
