# # Closures . 👋

### 1. What are IIFE ?
```bash
=> An IIFE (Immediately Invoked Function Expression) is a JavaScript function that runs as soon as it is defined.
    (function (){ 
    // Function Logic Here. 
    })();
```
### 1. What is currying ?
```bash
 -> Currying is a technique of evaluating function with multiple arguments, into sequence of functions with single argument.In other words, when a function, instead of taking all arguments at one time, takes the first one and return a new function that takes the second one and returns a new function which takes the third one, and so forth, until all arguments have been fulfilled.
 => Example .

    In the following example,since no currying is used, all the parameters were passed at once(volume(11,2,3))  to the existing function to calculate the volume.

    <html>
    <body>
    <script>
    function volume(length, width, height) {
        return length * width * height;
    }
    document.write((volume(11,2,3)));
    </script>
    </body>
    </html>
```
### 1. Write a program to throttle using closures ?
```bash
 ...Answer
```