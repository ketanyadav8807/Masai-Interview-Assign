### 1. Give an example where call apply bind is. required ?

```bash
    Answer ...
```
### 2. What is the difference between readFile and readFileSync ?

```bash
   => readFileSync() is synchronous and blocks execution until finished. These return their results as return values.
   => readFile() are asynchronous and return immediately while they function in the background. You pass a callback function which gets called when they finish.
```
### 3. What does process in node.js mean ?

```bash
    => * The process object is the global object in Node. It can be accessed from anywhere; 
    * it is an instance of  EventEmitter. Each Node.js has a set of built-in functionality, accessible through the global process object.
    => The process object provides the standard input/output (stdio) streams stdin, stdout and stderr (as in C/C++) as in the following:

## stdin: a readable stream for reading input from the user.
## stdout: a writable stream, either synchronously or asynchronously.
## stderr: a blocking synchronous writable stream intended for error messages.
```
### 4. Explain what node.js is ?

```bash
* Node.js was developed by Ryan Dahl in 2009
    * Node.js is an open-source, cross-platform, back-end JavaScript runtime environment that runs on the V8 engine and executes JavaScript code outside a web browser. Node.js lets developers use JavaScript to write command line tools and for server-side scripting—running scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. Consequently, Node.js represents a "JavaScript everywhere" paradigm,[6] unifying web-application development around a single programming language, rather than different languages for server-side and client-side scripts.
```
### 5. What is the difference of JS from browser to JS on node.js ?

```bash
* Both the browser and Node.js use JavaScript as their programming language.
* Building apps that run in the browser is a completely different thing than building a Node.js application.
    => JavaScript is a programming language, which runs in web browsers. Whereas Node.js is an interpreter or running environment for JavaScript, which holds a lot of requiring libraries and all.
```
### 6. Write three different ways to reverse a string in Javascript? a. using inbuilt method, b. iteratively, c. recursively ?

```bash
    a. Using inbuilt method.

        let a = "Masai"
        console.log(a.split("").reverse().join(""));

    b. Iteratively.

        let a = "Masai";
        a = a.split("");
        
        let start = 0;
        let end = a.length-1;

        while(start < end){
            let temp = a[start];
            a[start] = a[end];
            a[end] = temp;
            start ++;
            end --;
        }

        console.log(a.join(""));

    c. recursively.
```
### 7. Write a program to check two objects are equal ( deep equal ) ?

```bash
    Answer ...
```
### 8. What is shallow equal ?

```bash
    Answer ...
```
### 9. Using classes write a program to build a Parking Lot ?

## Problem

*   Design a parking lot that can be used for parking vehicles
*    The parking lot should have multiple floors where customers can park their cars.
* Customers should be able to purchase a parking ticket
* Parking lot has a maximum capacity
* Each parking floor will have many parking spots.
* The system should support parking for different types of vehicles

## There are four types of users here

* Admins
* Users
* Parking assistant

## Features

* CRUD - parking floor
* CRUD - parking spot
* CRUD - parking assistant
* Create a new parking ticket for customers
* Scan tickets to retrieve total value
* Pay

```bash
    Answer ...
```