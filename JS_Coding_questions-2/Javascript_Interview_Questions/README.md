## # Javascript Interview Questions . 👋
## # Problem ? 🚀

### 1. What is hoisting ?

```bash
 * Hoisting was thought up as a general way of thinking about how execution contexts (specifically the creation and execution phases) work in JavaScript.
 * JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to execution of the code.

 # Function hoisting
    => One of the advantages of hoisting is that it lets you use a function before you declare it in your code.

        catName("Tiger");

        function catName(name) {
        console.log("My cat's name is " + name);
        }
        /*
        The result of the code above is: "My cat's name is Tiger"
        */

 # var hoisting
    => Here we declare then initialize the value of a var after using it. The default initialization of the var is undefined .

        console.log(num); // Returns 'undefined' from hoisted var declaration (not 6)
        var num = 6; // Initialization and declaration.
        console.log(num); // Returns 6 after the line with initialization is executed.

 # let and const hoisting
    => Before Assigning some value let and const be in temporal dead zone , it does'nt assign with undefined as default value .Variables declared with let and const are also hoisted but, unlike var, are not initialized with a default value. An exception will be thrown if a variable declared with let or const is read before it is initialized.

    console.log(num); // Throws ReferenceError exception as the variable value is uninitialized
    let num = 6; // Initialization

 # class hoisting
    => Classes defined using a class declaration are hoisted, which means that JavaScript has a reference to the class. However the class is not initialized by default, so any code that uses it before the line in which it is initialized is executed will throw a ReferenceError.
```
### 2. What is scoping ?

```bash
 * Scope determines the accessibility (visibility) of variables.
 *JavaScript has 3 types of scope:-
    1. Block scope
    2. Function scope
    3. Global scope

  * "Before ES6 (2015), JavaScript had only Global Scope and Function Scope".
  * "ES6 introduced two important new JavaScript keywords: let and const."
  * "These two keywords provide Block Scope in JavaScript."
  # Block Scope 
    => Variables declared inside a { } block cannot be accessed from outside the block:-
        {
            let x = 2;
        }
        // x can NOT be used here

  * "Variables declared with the var keyword can NOT have block scope.
    Variables declared inside a { } block can be accessed from outside the block."

        {
            var x = 2;
        }
        // x CAN be used here

 # Local Scope 
    => Variables declared within a JavaScript function, become LOCAL to the function.

        // code here can NOT use carName

        function myFunction() {
            let carName = "Volvo";
            // code here CAN use carName
        }

        // code here can NOT use carName

 * "Local variables have Function Scope:
    They can only be accessed from within the function."
    # Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.
    # Local variables are created when a function starts, and deleted when the function is completed.
 * Function Scope
    => * "JavaScript has function scope: Each function creates a new scope."
       * "Variables defined inside a function are not accessible (visible)     from outside the function."
       * "Variables declared with var, let and const are quite similar when declared inside a function."

    1. function myFunction() {
         var carName = "Volvo";   // Function Scope
       }
    2. function myFunction() {
         let carName = "Volvo";   // Function Scope
       }
    3. function myFunction() {
         const carName = "Volvo";   // Function Scope
       }

    "They all have Function Scope:"

 * Global Scope
    => * Variables declared Globally (outside any function) have Global Scope.
       * Global variables can be accessed from anywhere in a JavaScript program.
       * "Variables declared with var, let and const are quite similar when declared outside a block".
       * "They all have Global Scope":

    let carName = "Volvo";
    // code here can use carName

    function myFunction() {
    // code here can also use carName
    }

    var x = 2;       // Global scope
    let x = 2;       // Global scope
    const x = 2;     // Global scope
```
### 3. How are var, let const different ?

```bash
 Answer will be updated soon . ...
```

### 4. What are the two main differences in arrow functions ?

```bash
 Answer will be updated soon . ...
```