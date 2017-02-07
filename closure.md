Closure:


Closures are free variables. Closures are the variables that can be used locally but defined in outer scope. In other words, closure
is a private or local function that has access to outer function's variable.
Also, global variables can be made private or local with the help of closure.
A closure has access to its own scope as well as access to outer function's variables. These functions remember the environment in which they are created.
Moreover, it has access to global variable too. 

Example:


function printname(first,last){
    let name="Your name is";
    function fullname(){
        return name+first+"  "+last;
    }
    return fullname();
}

name("Komal","Heer");


It has access to outer function's variables even after outer function returns a value or the outer function has been closed. It also stores references
to other function's variables.

Closures are used for data privacy, in callback functions, in event handlers and other programming patterns.

More about  Closures:



A closure is group of enclosed functions with references to its surrounding or lexical environment.
In Javascript, closures are created every time a function is created. To use a closure, a function is created inside other function and then it is passed or 
returned to another function.
Then, the inner function has access to outer function's scope, even after the outer function has been returned.






References:


http://javascriptissexy.com/understand-javascript-closures-with-ease/
http://www.w3schools.com/js/js_function_closures.asp
https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36#.9q9ylv6q8