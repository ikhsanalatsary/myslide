+++

title = "JavaScript"
weight = 2
date = "2017-04-24T18:36:24+02:00"
type="slide"

theme = "league"
[revealOptions]
transition= 'convex'
controls= true
progress= true
history= true
center= true
+++

## Introduction and The Goal of This Section

---

### Pengenalan & Tujuan

- Mengenal JavaScript
- Memahami karakteristik dan konsep
- Memahami sintaks

---

## Setup

- Text Editor menggunakan Brackets
- Browser menggunakan Chrome
- Developer tools Chrome

---

## Project Download

[Learn JavaScript](https://goo.gl/dhxycF)

---

#  Apa itu JavaScript

___

## JavaScript

JavaScript adalah cross-platform, bahasa scripting berorientasi objek. (MDN-Mozilla)

---

# JavaScript Dan Java

___

JavaScript Bukan Java. namun sintaks javascipt mirip java dalam beberapa case tertentu.

---

## Conceptual Aside

<ul>
  <li class="fragment fade-up">Syntax Parsers</li>
  <li class="fragment fade-up">Execution Contexts</li>
  <li class="fragment fade-up">Lexical Environments</li>
</ul>

---

## Syntax Parsers:

### A PROGRAM THAT READS YOUR CODE AND DETERMINES WHAT IT DOES AND IF ITS GRAMMAR IS VALID

<p class="fragment fade-up">Your code isn't magic. Someone else wrote a program to translate it for the computer.</p>

---

<!-- ![Syntax Parser](/myslide/intro-to/syntaxparser.jpeg) -->
<img src="/myslide/intro-to/syntaxparser.jpeg" width=800 alt="Syntax Parser" />

---

## Lexical Environment:

### WHERE SOMETHING SITS PHYSICALLY IN THE CODE YOU WRITE

<p class="fragment fade-up">'Lexical' means 'having to do with words or grammar'. A lexical environment exists in programming languages in which where you write something is important.</p>

---

## Execution Contexts:

### A WRAPPER TO HELP MANAGE THE CODE THAT IS RUNNING

<p class="fragment fade-up">There are a lots of lexical environments. Which one is currently running is managed via execution contexts. it can contain things beyond what you've written in your code.</p>

---

# It's Important!

---

## Conceptual Aside:

### Name / Value Pairs And Objects

___

## Name / Value Pair:

### A NAME WHICH MAPS TO A UNIQUE VALUE

<p class="fragment fade-up">The name may be defined more than once, but only can have one value in any given context.<br />
That value may be more name/value pairs.</p>

___

## For Example

`Alamat = 'Jl. Margonda no. 7'`

---

## Object:

### A COLLECTION OF NAME VALUE PAIRS

<p class="fragment fade-up">The simplest definition when talking about JavaScript.</p>

___

## Ilustration

![Syntax Parser](/myslide/intro-to/name-value-pairs.jpeg)

___

## Example Object

```javascript
{
  Alamat:
    {
      Jalan: 'Margonda',
      Nomor: 7,
      Apartemen:
      {
        Lantai: 3,
        Nomor: 007
      }
    }
}

```

---

## The Global Environment And The Global Object

___

### Execution Context (Global)

* Global Object
* `this`

<p class="fragment fade-up">
  <img src="/myslide/intro-to/execution-context.jpeg" alt=" execution context"/>
</p>

---

# Let's start code!

---

# So...

---

## Global Object adalah `Window`

Global Object(`window`) sama dengan `this`

<p class="fragment fade-up">
  <img src="/myslide/intro-to/execution-context-equal.jpeg" alt="execution context equal" />
</p>

---

## Global

- **Not inside a `function`**

---

![execution context final](/myslide/intro-to/execution-context-final.jpeg)

---

## Creation and Hoisting

___

![Creation and Hoisting](/myslide/intro-to/creation-hoisting.jpeg)

---

## Conceptual Aside:
## JavaScript and `undefined`

___

![JavaScript and undefined](/myslide/intro-to/javascript-undefined.jpeg)

---

## The Execution Context - Code Execution

___

![JavaScript and undefined](/myslide/intro-to/code-execution.jpeg)

---

## Conceptual Aside
### Single Threaded
### Syncronous Execution

___

## Single Threaded:
### One Command at a time

<p class="fragment fade-up">
  Under the hood of the browser, maybe not
</p>

___

## Syncronous:
### One at a time

---

## Function Invocation
## And
## The Execution Context

---

## Invocation:
### Running A Function

<p class="fragment fade-up">
  In JavaScript, by using parenthesis `()`
</p>

---

## Execution Stack

![Invocation1](/myslide/intro-to/invocation1.gif)

___

## Execution Stack

<img src="/myslide/intro-to/execution-stack.gif" width=800 alt="Execution Stack" />

___

## Execution Stack

<img src="/myslide/intro-to/execution-stack-1.gif" width=800 alt="Execution Stack" />

---

## Function, Context, and Variable Environment

---

## Variable Environment:
### Where the variable live

<p class="fragment fade-up">
  And how they relate to each other in memory
</p>


---

## Scope Chain

<img src="/myslide/intro-to/scope-chain.gif" width=800 alt="Execution Stack" />

---

## Conceptul Aside
### Types And JavaScript

___

## Dynamic Typing:
### You don't tell the engine what type of data a variable holds, it figures it out while your code is running

<p class="fragment fade-up">
  Variables can hold different types of values because it's all figured out during execution
</p>

___

## Static Typing

```java
  bool isNew = 'hello'; // an error
```

## Dynamic Typing

```javascript
  var isNew = true; // no errors
  isNew = 'yup!';
  isNew = 1;
```

---

## Primitive Type:
### A Type of data that represents a single value

<p class="fragment fade-up">
  That is, not an object
</p>

---

## Undefined

<p class="fragment fade-up">
  `undefined` represents lack of existence
  (you shouldn't set a variable to this)
</p>

---

## Null

<p class="fragment fade-up">
  `null` represents lack of existence
  (you can set a variable to this)
</p>

---

## Boolean

<p class="fragment fade-up">
  `boolean` is true or false
</p>

---

## Number

<p class="fragment fade-up">
  *Floating point* number (there's always some decimals). Unlike other programming languages, there's only one `number` type. and it can make math weird.
</p>

---

## String

<p class="fragment fade-up">
  a sequence of characters
  (both '' and "" can be used)
</p>

---

## Symbol

<p class="fragment fade-up">
  Unique type. Used in ES6 (the next version of JavaScript)
</p>

---

## Conceptual Aside:
### Operators

---

## Operator:
### A Special Function That is Syntactically (Written) Differently

<p class="fragment fade-up">
  Generally, Operators take two parameters and return one result
</p>

---

## Conceptual Aside:
### Coercion

---

## Coercion
### Converting a value from one type to another

<p class="fragment fade-up">
  This Happens quite often in JavaScript because it's dynamically typed.
</p>

---

## Default Value

let's code

---

## Operator Precedence And Associativity

---

## Operator Precedence:
### Which Operator function gets called first

<p class="fragment fade-up">
  Functions are called in order of precedence (Higher precedence wins)
</p>

---

## Associativity:
### What Order Operator Functions Get Called In:
### Left-To-Right or Right-to-left

<p class="fragment fade-up">
  When functions have the same precedence
</p>

---

## Comparison Operators

let's code

---

## Objects And Functions

---

## Object And The Dots

___

![Objects and the dots](/myslide/intro-to/objects-dots.jpeg)

___

![Objects and the dots in memory](/myslide/intro-to/objects-dots-memory.jpeg)

---

## Object Literals

---

## Faking NameSpace

---

## JSON & Object literals

---

## function are Objects

---

## function statements and function expression

---

## Object, function and `this`
---

## by value and by reference

---

## Conceptual Aside:
## Array

<p class="fragment fade-up">
  Collections of anything
</p>

## Conceptual Aside:
## Building Objects

___

## Function Constructors, new, and the history of JavaScript

let's code after cerita dulu

___

## Function Constructors:
### A normal Function that is used to construct objects.

<p class="fragment fade-up">
  The `this` variable points a new empty object, and that object is returned from the Function automatically.
</p>

---

## Conceptual Aside:
## Event:
### Something that has happened in our app that we can respond to
