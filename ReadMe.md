## Javascipt Scope
The scope is what defines the access to javascript variables. In javascript, variables can belong to the global scope or to the local scope. Global variables are variables that belong in the global scope and are accessible from anywhere in the program.

## Responsive Web Design
Responsive Web Design is about creating web sites which automatically adjust themselves to look good on all devices, from small phones to large desktops.

## Scope - Var Keyword
When we declare a variable that variable should only be accessible in the block in which it's define, this is what we called Scope.

When we declare a variable with "var" keyword that variable is accessible inside of the function in which it's define

## Let 
When we declare a variable with let keyword that variable is only accessible inside of that block in which it's define.

## var -> Variables declared with var keyword are scope to the function. The most common variable. It can be reassigneed but only accessed withing a function. Variables defined with var keyword move to the top when the code is executed.

## let -> Variables declared with let keyword are scoped to the block in which they are define. Use let only when reassign a variable but not redeclare.

## const -> const is defined to constant, very similar to let keyword, const is also a block scope in which they are define. Not accessible before they appear within the code

## The difference between 'const ' and 'let'
 can reassigned a variable with let keyword
 cannot reassigned a variable with const keyword

## Objects -> objects in javascript are collections of key value pairs. In Object Oriented programming term if we have function inside of an object we referred to that function as a method

## Strict Mode
The mode to execute a javascript code in more protective way so it prevents potential problem, thats why in this case instead of getting a reference to a window object we get undefined

## 'this' is determined by how a functon is called.
If we called a function as a method in an object this will always return a reference to the current object.

However, If we call a function as a standalone object or outside of an object this will result as a global object, which is window object in a browser

But in react the result is undefined because the strict mode is enabled by default.

## Binding 'this' ->
In Javascript, functions are an object. 'bind' is method and we can use this method to bind a function to an object
With bind method we can set value of this permanantaly
  
## Arrow Function ->
They don't rebind this keyword
If we change a function to arrow function it will inherit 'this' keyword
When we use function keyword in callback function will get window object.
And we use Arrow function in callback function will get reference to the whatever object is.
==========================================================

A computer, a compiler or even a browser can't actually 'understand' code that's written  in JS, if so how does the code run?

Behind the scenes, JS always runs in certain enviroment, most common ones are:
1. Browser (by far the most common)
2. Node.js (Which is a runtime enviroment which allows you to run JS outside of the browser, usually in servers)

JS needs to run in a certain enviroment, but what exactly is in the eviroment?

When you write code in js, you write it in human-readable syntax, with alphabets and numbers. As mentioned, a machine can not understand this type of code.

This is why each environment has an engine. 

In general, the engine's job is to take that code and transform it into machine code which can eventually be run by the computer processor.

Each environment has its own engine, the most common ones are Chorme V8( Which Node also uses), Firefox SpiderMonkey, JavascriptCore by safari and Chakra By IE

All engine works in similar fasion but there are differences between each engine

It's also important to keep in mind that behind the scenes an engine is simply software, Chrome V8 for example is a software writte in C++.
===========================================================
A Parser is a compiler or interpreter component that breaks data into smaller elements for easy translation into another language. A parser takes input in the form of a sequence of tokens, interactive commands, or programm instructions and breaks them up into parts that can be used by the other components in programming.
===========================================================

We have an environment, and we have an engine inside that environment. The first thing the engine does upon executing your code is check the code using the parser.

The parser knows JS syntax and rules, and its job is to go through the code line by line and check if the syntax of the code is correct.

If the parser comes across an error, it stops running and sends out an error. If the code is valid, the parser generates somthing that's called an Abstract Syntax Tree.

So our environment has an engine, which has a parser, which generates an AST. What is ast

AST is a data structure, which is not unique to JS but actually used by a lot other language.
An AST is simply tree representation of your code, and the main reason the engine creates an AST instead of compiling directly to a machine code is that it's easier to covert to machine code when you have the code inside a tree data structure

The interpreter's job is to take the AST that has been created and transform it into Intermediate Representation of the code.

An IR is a data structure or code which represents the source code. Its role is to be an intermediate step between code that's written in an abstract langauge such as js and machine code
===========================================================

The "appendChild()" method appends a node as the last child of a node.
Tip: If you want to create a new paragraph, with the text, remember to create the text as a Text Node which you append to the paragraph, then append to the paragaph to the document.
You can also use this method to move an element from one element to another.
Tip: Use the insertBefore() method to insert a new child node before a specified, existing, child node 
===========================================================
What is Closure?
    A closure is a function plus a connection to the variables that exist at its "birth place".

What is the point of keeping this connection?
    It provides the values for the free variables of the function
===========================================================

Regular function and Arrow function difference

1) Syntax : reg use function keyword and arrow use => arrow

2) this keyword : reg have its own this context and arrow don't have thier own this context.

3) new keyword : reg is constructible and callable can call using new keyword
and arrow is not contstructible but callable but due to which will get runtime error when trying to construct non-constructible arrow function using new.
============================================================
MVC ->
1) Model - Manages data and business logic
2) View - Handles layout and display
3) Controller - Routes commands to the model and view parts