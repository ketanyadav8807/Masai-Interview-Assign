# # Node Interview Questions . 👋

### 1. Explain in brief what is node js ?
```bash
 ...Answer
```
### 2. How is node js non blocking ?
```bash
=> Blocking === Synchronous .
 - line by line execution .
 - Blocking: It refers to the blocking of further operation until the current operation finishes.
 - Blocking methods are executed synchronously. Synchronously means that the program is executed line by line. The program waits until the called function or the operation returns.
 - uses the readFileSync() function to read files and demonstrate Blocking in Node.js
=> Non Blocking === Synchronous .
 - line by line execution not guaranteed .
 - Non-Blocking: It refers to the program that does not block the execution of further operations. Non-Blocking methods are executed asynchronously. Asynchronously means that the program may not necessarily execute line by line. The program calls the function and move to the next operation and does not wait for it to return.
 - uses the readFile() function to read files and demonstrate Non-Blocking in Node.js
```
### 3. What is throughput ?
```bash
=> The amount of Data Transfered from client to server in a given time period is called Data Throughput .
 - In communication networks, network throughput (or just throughput, when in context) is the rate of successful message delivery over a communication channel, such as Ethernet or packet radio. The data these messages belong to may be delivered over a physical or logical link, or it can pass through a certain network node. Throughput is usually measured in bits per second (bit/s or bps), and sometimes in data packets per second (p/s or pps) or data packets per time slot.
 - The system throughput or aggregate throughput is the sum of the data rates that are delivered to all terminals in a network.[1] Throughput is essentially synonymous to digital bandwidth consumption; it can be analyzed mathematically by applying the queueing theory, where the load in packets per time unit is denoted as the arrival rate (λ), and the throughput, where the drop in packets per time unit, is denoted as the departure rate (μ).
 - The throughput of a communication system may be affected by various factors, including the limitations of underlying analog physical medium, available processing power of the system components, and end-user behavior. When various protocol overheads are taken into account, useful rate of the transferred data can be significantly lower than the maximum achievable throughput; the useful part is usually referred to as goodput.
```
### 4. How is Node js having high IO throughput ?
```bash
 ...Answer
```
### 5. What are CPU intensive tasks ?
```bash
 ...Answer
```
### 6. How can you end up blocking your main thread in node.js ?
```bash
 ...Answer
```
### 7. What is the event loop ?
```bash
=> The event loop is the secret by which JavaScript gives us an illusion of being multithreaded even though it is single-threaded .
=> allback function in the event queue has not yet run and is waiting for its time into the stack when the SetTimeOut() is being executed and the Web API is making the mentioned wait. When the function stack becomes empty, the function gets loaded onto the stack .
=> That is where the event loop comes into picture, it takes the first event from the Event Queue and places it onto the stack .
```
### 8. What are different phases in event loop ?
```bash
 => The Event Loop contains six main phases: timers, I/O callbacks, preparation / idle phase, I/O polling, setImmediate() callbacks execution, and close events callbacks.
 => After a phase is complete, the application moves to the next tick and all phases are repeated again starting with timers until there is nothing left to process
```
### 9. What is process.tick ?
```bash
=> Every time the event loop takes a full trip, we call it a tick.
=> Calling setTimeout(() => {}, 0) will execute the function at the end of next tick, much later than when using nextTick() which prioritizes the call and executes it just before the beginning of the next tick. REF:- https://nodejs.dev/learn/understanding-process-nexttick

Source :- GFG:- https://www.geeksforgeeks.org/nodejs-process-nexttick-method/
=>  In the code of snippet, the second console is printed first because this is a part of the current iteration of the event loop, and the first console is a part of a callback function that is associated with the process.nextTick() executed in the next iteration of the event loop.
Below examples illustrate the use of the process.nextTick() property in NodeJS:

Example:

// Node.js program to demonstrate the
// process.nextTick() Property
	
// Include process module
const process = require('process');

process.nextTick(() => {
console.log('Executed in the next iteration');
});

console.log('Executed in the current iteration');

```
### 10. When can process.tick starve your event loop ?
```bash
 ...Answer
```
### 11. What is the difference between setTimeout and setInterval ?
```bash
 setTimeout will be triggered once after interval of time . But the setInterval keeps trigering expression regularly after a given interval of time.
```
### 12. How can you make a network request with http module from the backend ?
```bash
 ...Answer
```
### 13. How can you create your own events ?
```bash
 ...Answer
```
### 14. What are clusters ?
```bash
 ...Answer
```
### 15. How does your Node.js application handle scale? Elaborate ?
```bash
 ...Answer
```
### 16. What is the difference between readFile and readFileSync ?
```bash
 ...Answer
```
### 17. What are CORS? How do you configure them? Why do you need them ?
```bash
 ...Answer
```
### 18. What is rate limiting ?
```bash
 ...Answer
```
### 19. How does middlewares work in express ?
```bash
 ...Answer
```
### 20. What is the difference between Encryption and Hashing ?
```bash
 ...Answer
```
### 21. What is the difference between https and http ?
```bash
 ...Answer
```
### 22. What is TLS ?
```bash
 ...Answer
```
### 23. What is AES ?
```bash
 ...Answer
```
### 24. What is JWT Token? Why do we need to use JWT? What are some pros and cons ?
```bash
 ...Answer
```
### 25. What is salting? Where do we store salt ?
```bash
 ...Answer
```
### 26. What is the difference between Authorisation and Authentication ?
```bash
 * authentication is the process of verifying who someone is, whereas
 *  authorization is the process of verifying what specific applications, files, and data a user has access to
```
### 27. What is difference between JS on the browser and node ?
```bash
=> Node js has full access to the system whereas for the browser is get access to the given files.
```
### 28. What is V8 ?
```bash
 V8 is a free and open-source JavaScript engine developed by the Chromium Project for Google Chrome and Chromium web browsers. The project’s creator is Lars Bak. The first version of the V8 engine was released at the same time as the first version of Chrome: 2 September 2008.
```
