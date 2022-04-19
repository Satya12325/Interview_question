# Explain in brief what is node js?
Ans- Node. js (Node) is an open source development platform for executing JavaScript code server-side. Node is useful for developing applications that require a persistent connection from the browser to the server and is often used for real-time applications such as chat, news feeds and web push notifications.
# How is node js non blocking?
Ans- Non-Blocking: 
It refers to the program that does not block the execution of further operations. Non-Blocking methods are executed asynchronously. Asynchronously means that the program may not necessarily execute line by line. The program calls the function and move to the next operation and does not wait for it to return.

Example: Following example uses the readFile() function to read files and demonstrate Non-Blocking in Node.js

const fs = require('fs');
   
const filepath = 'text.txt';
  
// Reads a file in a asynchronous and non-blocking way 
fs.readFile(filepath, {encoding: 'utf8'}, (err, data) => {
    // Prints the content of file
    console.log(data);
});
  
  
// This section calculates the sum of numbers from 1 to 10
let sum = 0;
for(let i=1; i<=10; i++){
    sum = sum + i;
}
  
// Prints the sum
console.log('Sum: ', sum);

# What is throughput?

Ans- Throughput is a measure of how many units of information a system can process in a given amount of time. It is applied broadly to systems ranging from various aspects of computer and network systems to organizations. Related measures of system productivity include the speed with which some specific workload can be completed, and response time, the amount of time between a single interactive user request and receipt of the response.  

# what is bandwidth?
bindwidth tells you how much data could theoretically be transferred from a source at any given time.

Speed is one of the most important things used to measure network performance, and we use throughput and bandwidth to measure it.

# How is Node js having high IO throughput?
Server side caching is one of the most common strategies for improving the performance of a web application. it's primary aim is to increase the speed of data retrieval, either by spending less time computing such data or doing I/O.

# What are CPU intensive tasks?
CPU intensive tasks will block all request from completing, untill the task is completed.

# How can you end up blocking your main thread in node.js?
if a server request to do calculations that will take some time of complete . will doing a setTimeout(()=>{ write logic here....... },time)

# What is the event loop?
event loop which is responsible for executing the code allows us to use callback and promises;

Due to fact that js is single threaded it performs only a single process at a time. so it is the event loop that allows node.js to perform non-blocking I/O operations.

let take a example of event loop console.log("1st") setTimeout(()=>{ console.log("2nd"); },2000); console.log("3rd");

# What are different phases in event loop?
Event loop contains six main phases:

timer,
I/O callbacks,
prepration / idle pahase
I/O polling
setImmediate() callbacks execution,
close event callbacks.

# What is process.tick?
it's help to excute next callback function.
process.nextTick() is used to schedule a callback function to be invoked in the next iteration of the Eventloop.

# When can process.tick starve your event loop?
process.nextTick() function is specific to the Node.js Event Loop

# What is the difference between setTimeout and setInterval?
setTimeout() triggers the expression only once while setInterval() keeps triggerring expression regularly after the given interval of time.

# How can you make a network request with http module from the backend?
const http = require("http"); const server = http.createServer((req,res)=>{ res.write('HEllo duniya'); // write responce for client res.end(); // end response });

server.listen(8000,()=>{ console.log('server is working'); })

# What are clusters?
a computer cluster is a group of two or more computer or nodes, that run in parallel to achieve a common goal.

# How does your Node.js application handle scale? Elaborate
Scalability is built in the very core of the runtime.
Horizontally scalling a node.js application

# What are CORS? How do you configure them? Why do you need them?
cors is builtin middleware basiclly it's help conncet fronted to backend.

# What is rate limiting?
Rate limiting is a strategy for limiting network traffic. it puts a cap on how often someone can repeat an action within a certain timeframe.

# How does middlewares work in express?
functions that have access to the request object and response object and the next function in the application's request-responce cycle.

the next function is a function in the express router which, when invoked, executes the middleware succeeding the current middleware.

# What is the difference between Encryption and Hashing?
encryption is a two-way function that includes encryption and decryption

hashing is a one-way function that changes a plain text to a unique digest that is irreversible.

# What is the difference between https and http?
Both are protocols of a perticular website is exchanged between Web Server and Web Browser.

https is much more secure compared to http.

# What is TLS?
Transport Layer Security => encrypts data sent over the internet to ensure that hackers are unable to see what you transmit

# What is AES?
Advanced Encryption Standard is used to order to protect data against unauthroised access and to encrypt this. The cryptographic process key of varying lengths is utilised for this purpose.

# What is JWT Token? Why do we need to use JWT? What are some pros and cons?
pros => Simpler to use if careful => used cross service you can have one authorization server that deals with the login/ Registration and generates the token,.
const => compromised secreat key => if key is leaked by a careless or a rouge developer/ administrator the whole system is compromised.

# What is salting? Where do we store salt?
the salt is not an encryption key. so it can be stored in the password database along with username.

# What is the difference between Authorisation and Authentication?
authentication is the process of verifying who is someone.
authorization is the process of verifying what user has access to file or data..........

# What is difference between JS on the browser and node?
js and chrome is both v8. so many of the node.js features are not available in a browser context.

# What is V8?
V8 provides the runtime environment in which js executes. V8 is the name of the JavaScript engine that powers Google Chrome.