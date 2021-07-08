### Context and 'this' Keyword

![regina george exclaiming 'what is this?'](https://media.giphy.com/media/xT9KVAk831VqO2bmWk/giphy.gif)

---

By the end of this lesson, you will be able to...

- explain what 'this' is in JavaScript
- determine what 'this' is referring to in a codebase

---

#### Vocab

invoke/execution

---

#### Define: 'this' in a sentence...

'this' is just a placeholder for the context that called the function.
In other words, the this references the object that is currently calling the function.

But what does that actually mean?
<!-- .element: class="fragment" -->

Notes: 
rephrase several times: 
this is the context of a function invocation
this refers to the object that the function belongs to
A property of an execution context (global, function or eval) that is always a reference to an object.

Analogies: 
I just started cutting an onion. _Where_ I started cutting an onion might be my 'this' (Kitchen.chop())

I'm learning calculus. The major I'm in might be my 'this'

---

Go through some examples and define a few rules that apply to the keyword this...

[sandbox](https://codesandbox.io/s/context-and-this-keyword-lbwst?file=/src/index.js)

```
class Unicorn {
  constructor(name, color) {
    // What is logged here?
    console.log(this);  

    this.name = name;
    this.color = color;

    // What changes about "this"?
    console.log(this);  
  }

  says() { 
    console.log(`${this.name} is my favorite ${this.color} pony`, this);
  }
}
```

---

Rule #1
'this' within function code invoked using the new operator refers to the new instance of that object.

---

Rule #2
When executing a function as a method on an object, 'this' refers to that object.

---

To confirm these theories, consider the following example...

Write your answers down.

---

What is the value of 'this'?
When is the value of 'this' set?

```
function logThis() {
  console.log(this);
}

const voyager1 = {
  classification: 'Space Probe',
  title: 'Voyager 1',
  logThis: logThis
}

const voyager2 = {
  classification: 'Space Probe',
  title: 'Voyager 2',
  logThis: logThis
}

voyager1.logThis(); 
voyager2.logThis();
```

---

A common way to think about 'this':

If a function is executed and there is a . before the name of the function, 'this' refers to whatever comes before the .

```

Unicorn.say();

```

---

Practice in Pairs: 

[sandbox](https://codesandbox.io/s/context-and-this-keyword-2-43gqi?file=/src/index.js)

---

What is the default value of 'this'?

```
function logThis() {
  console.log(this);
}

logThis();
```

---

Rule #3
By default, this refers to the global object (or in the browser, the window).

---

... except when we are in strict mode...

```
"use strict";

function logThis() {
  console.log(this);
}

logThis();
```

(If your program is running in strict mode and neither of the first two rules apply, then this will be undefined.)
<!-- .element: class="fragment" -->

---

For our purposes here, these are the three main rules that this follows. You might find exceptions out there especially when looking at ways that you can explicity change the value of this using methods like call, apply, or bind, but we’ll cover this another time!

---

Rule #1

'this' within function code invoked using the new operator refers to the new instance of that object.
<!-- .element: class="fragment" -->

---

Rule #2

When executing a function as a method on an object, 'this' refers to that object.
<!-- .element: class="fragment" -->

---

Rule #3

By default, this refers to the global object (or in the browser, the window).
<!-- .element: class="fragment" -->

---

Arrow functions and 'this'

If you are unfamiliar with arrow functions, find more info in the es5 vs es6 lesson. 

```
() => {}
```

Try it out in pairs: [sandbox](https://codesandbox.io/s/context-and-this-keyword-4-050ky)

Notes:
When considering using a traditional function vs an arrow function note that:
function () {}: The value of this is set when the function is executed.
() => {}: The value of this is set when the function is created.

---

Different terms of art...

Many sources will use the terms 'explicit', 'default' and 'implicit' _bindings_.

In non-strict mode...
- Default binding is the global object
- Implicit binding is the object within which the function was called
- Explicit binding is to force the function to use a certain object as its 'this'.

---

Check for understanding:

What is 'this' in JavaScript?
<!-- .element: class="fragment" -->

What are the rules for determining 'this'?
<!-- .element: class="fragment" -->
