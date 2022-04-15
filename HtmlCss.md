Explain briefly what happens when you hit a url?
Ans: -Browser initiates TCP connection with the server. Browser sends the HTTP request to the server.
 Server processes request and sends back a response. Browser renders the content
 DNS lookup :- DNS Stands for (omain Name System)Web browsers interact through Internet Protocol (IP) addresses. DNS translates domain names to IP addresses so browsers can load Internet resources.


# What is HTTP protocol?

 HTTP is a protocol for fetching resources such as HTML documents. It is the foundation of any data exchange on\
  the Web and it is a client-server protocol

# What is HTTPS?

Hypertext transfer protocol secure (HTTPS) is the secure version of HTTP, which is the primary 
protocol used to send data between a web browser and a website. HTTPS is encrypted in order to 
increase security of data transfer

# What is TCP Protocol? 

TCP stands for Transmission Control Protocol a communications standard that enables application programs and computing devices to exchange messages over a network. It is designed to send packets across the internet and ensure the successful delivery of data and messages over networks.
<img src="https://marvel-b1-cdn.bc0a.com/f00000000216283/www.fortinet.com/content/fortinet-com/en_us/resources/cyberglossary/tcp-ip/_jcr_content/par/c05_container_935138/par/c28_image_copy_copy_.img.jpg/1625683654934.jpg">

TCP use in :-  TCP enables data to be transferred between applications and devices on a network and is used in the TCP IP model. It is designed to break down a message, such as an email, into packets of data to ensure the message reaches its destination successfully and as quickly as possible.


# HTTP request methods:- 

# GET
The GET method requests a representation of the specified resource. Requests using GET should only retrieve data.

# GETHEAD
The HEAD method asks for a response identical to a GET request, but without the response body.

# POST
The POST method submits an entity to the specified resource, often causing a change in state or side effects on the server.

# PUT
The PUT method replaces all current representations of the target resource with the request payload.

# DELETE
The DELETE method deletes the specified resource.

# CONNECT
The CONNECT method establishes a tunnel to the server identified by the target resource.

# OPTIONS
The OPTIONS method describes the communication options for the target resource.

# TRACE
The TRACE method performs a message loop-back test along the path to the target resource.

# PATCH
The PATCH method applies partial modifications to a resource.

BAsically we use 6 methodes thees are 
# => GET, POST, PUT, PATCH, DELETE


# What are HTTP headers?

Ans - HTTP headers let the client and the server pass additional information with an HTTP request or response. An HTTP header consists of its case-insensitive name followed by a colon ( : ), then by its value. Whitespace before the value is ignored.


# What are some HTTP response codes?what does it mean?

HTTP response status codes
Informational responses ( 100 – 199 )
Successful responses ( 200 – 299 )
Redirection messages ( 300 – 399 )
Client error responses ( 400 – 499 )
Server error responses ( 500 – 599 )

# What does cache control on http response mean?

Ans - Cache-control is an HTTP header used to specify browser caching policies in both client requests and server responses. Policies include how a resource is cached, where it's cached and its maximum age before expiring.

# What is polling?

Polling is a technique where we check for fresh data over a given interval by periodically making API requests to a server. For example, we can use polling if there is data that changes frequently or we need to wait for the server to transition a given state.

# What is long polling?

Long polling is the simplest way of having persistent connection with server, that doesn't use any specific protocol like WebSocket or Server Side Events. Being very easy to implement, it's also good enough in a lot of cases.

# What are web sockets?
Ans- HTTP and WebSocket both are communication protocols used in client-server communication. 


# How is web sockets different from HTTP?

# web sockets:-

-WebSocket is a bidirectional communication protocol that can send the data from the client to the server or from the server to the client by reusing the established connection channel. The connection is kept alive until terminated by either the client or the server.

-All the frequently updated applications used WebSocket because it is faster than HTTP Connection.

# HTTP protocol - 

The HTTP protocol is a unidirectional protocol that works on top of TCP protocol which is a connection-oriented transport layer protocol, we can create the connection by using HTTP request methods after getting the response HTTP connection get closed.

-When we do not want to retain a connection for a particular amount of time or reuse the connection for transmitting data; An HTTP connection is slower than

 # What is HTTPS? 
 A. an internet communication protocol that protects the integrity and confidentiality of data between the user's computer and the site.

# What is Cross Origin Resource Sharing? ( CORS ) Why do we need it?
 A. allows you to make requests from one website to another website in the browser

# What does Access-Control-Allow-Origin header do?
 A. The Access-Control-Allow-Origin header is included in the response from one website to a request originating from another website, and identifies the permitted origin of the request.

# What is clickjacking? How do you fix it?
 A. Clickjacking is an attack that fools users into thinking they are clicking on one thing when they are actually clicking on another.

# What are some performance metrics for your website?
A.
Measure Your Audience’s Reach and Impact
Identify Your Traffic Sources
Measure Average Session Time and Bounce Rate
Measure Conversion Rates
Measure ROI and Profits
# What does the following term mean? 
Time to first byte => Time to First Byte (TTFB) refers to the time between the browser requesting a page and when it receives the first byte of information from the server.

Page load time => the average amount of time it takes for a page to show up on your screen. . It's calculated from initiation (when you click on a page link or type in a Web address) to completion (when the page is fully loaded in the browser).

# What do CDN or Content Delivery Networks do? When do you need a CDN?
 A. it's provide fast delivery of the internet content quick transfer of assets needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

# What is the difference between Client Side Renderring and Server Side Renderring? 
A. server-side rendering is able to display a fully populated page on the first load for any route of the website, whereas client-side rendering displays a blank page first.

# What is Progressive Renderring 
A. the technique of sequentially rendering parts of the web page on the server-side and send it to the client in portions without waiting for the entire page to be rendered.”

# What is the difference between Preloading and Prefetching resources? 

Preload is an early fetch instruction to the browser to request a resource needed for a page (key scripts, Web Fonts, hero images).

Prefetch serves a slightly different use case — a future navigation by the user (e.g between views or pages) where fetched resources and requests need to persist across navigations

# What are service workers?
 A. Service Worker is a script that works on browser background without user interaction independently. can track network traffic of the page, manage push notifications and develop “offline first” web applications with Cache API.