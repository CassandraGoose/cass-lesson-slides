# Object Literals

At the end of this lesson, you should be able to:
- explain the difference between dot notation and bracket notation
- identify scenarios that require bracket notation
- access and create key value pairs on complex data types

---

### Vocab review: 

- Object A bundle of behavior (methods) and state (properties)
- Key The name used to reference a value on an object
- Value The data referenced by a key
- Property How we refer to one of the key-value pairs of an object
- Method A function on an object
- Dot Notation Notation to access a value on an object, explicitly specifies the key

---

Review: What is an object anyways?

Answer the questions in the Zoom Poll!

Notes: 
BTW a literal is the actual value of the thing (notation for representing a fixed value). I prefer to think of it like this: it doesn't resolve to anything. it isn't an expression.

---

How do we access and create values? 

Dot and Bracket Notation. 

---

Dot Notation

```
const school = { name: 'Park Hill School' };
school.name // returns 'Park Hill School'
```

---

Bracket Notation

- Any expression can go inside the brackets
<!-- .element: class="fragment" -->

- JavaScript will evaluate what's inside the brackets before trying to create or access a key
<!-- .element: class="fragment" -->

- Knowing this, what might be a use case for using bracket notation? 
<!-- .element: class="fragment" -->

Note: 
Most common use-case is for dynamically accessing a property (think using an argument/parameter of a function to access a value, or variables or iterations)

It's also handy when your property name has weird characters like 'chicken-nugget' -> object['chicken-nugget']

---

```
let detail = 'coverLetter';

const developer = {
    name: 'Travis',
    experience: 3,
    coverLetter: true
};

developer[detail] // returns true
// detail will be evaluated and the interpreter will see
// that it represents a string of 'coverLetter' - so it will then
// look for a key of coverLetter in the developer object
```

Notes: 
Do the example with bits of a string spread out between variables and then access like developer[string1 + string2]
Questions?

---

[Pairs](https://codesandbox.io/s/object-literals-pair-work-m0q7m?file=/src/index.js)

Notes: for extra, have them drive you to modify a value because that's in the title but not anywhere in the official lesson

---

### You drive

```
const dog = {
  name: 'Boris',
  age: 3,
  breed: 'Pug'
};
```

We want to iterate through this object, grabbing the keys and values to log.

We want to log:

```
I have a dog and...
His name is Boris
His age is 3
His breed is Pug
```

Notes: 
there are several ways to do this:

```
const dog = {
  name: 'Boris',
  age: 3,
  breed: 'Pug'
};

// Object.keys gives us an array of the targeted object's keys
const dogDetails = Object.keys(dog); // ['name', 'age', 'breed'];

console.log('I have a dog and...');

for (let i = 0; i < dogDetails.length; i++) {
  console.log(`His ${dogDetails[i]} is ${dog[dogDetails[i]]}`);
}
```

---
Review!

Consider these questions for 15 seconds and then I will call on someone to answer. 

- When would you use dot notation?
<!-- .element: class="fragment" -->
- When would you use bracket notation?
<!-- .element: class="fragment" -->

---

[Practice](https://frontend.turing.edu/lessons/module-2/object-literals-accessing-creating-and-modifying-values.html)

BTW: It would be helpful to read up on the following Object methods: 
- Object.keys()
- Object.values()
- Object.entries()
- Object.assign()

---




