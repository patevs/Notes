# TypeScript Development Basics

> `TypeScript` is an open-source programming language developed and maintained by Microsoft. It is a strict syntactical superset of `JavaScript`, and adds optional static typing to the language.

- [Website](https://www.typescriptlang.org/)
- [Documentation](https://www.typescriptlang.org/docs/home.html)

---

## Links & Resources

- [`microsoft/TypeScript`](https://github.com/microsoft/TypeScript)
- [`microsoft/TypeScript-Node-Starter`](https://github.com/Microsoft/TypeScript-Node-Starter)
- [Quick Start Tutorial](https://www.typescriptlang.org/docs/tutorial.html)
- [TypeScript - JavaScript with SuperPowers](https://medium.com/better-programming/typescript-javascript-with-super-powers-a333b0fcabc9)

[](.)

- [`typescript-book`](https://github.com/basarat/typescript-book)
- [TypeScript Deep Dive](https://basarat.gitbooks.io/typescript/)

---

## Installation

For the latest stable version:

```bash
# Install globally
$ npm install -g typescript
# Check installation
$ tsc --version # or tsc -v
```

---

## Basic Examples

`greeter.ts`

```typescript
function greeter(person: string) {
    return "Hello, " + person;
}

var user = "Jane User";

document.body.innerHTML = greeter(user);
```

`greeter.html`

```html
<!DOCTYPE html>
<html>
    <head><title>TypeScript Greeter</title></head>
    <body>
        <script src="greeter.js"></script>
    </body>
</html>
```

Compile `greeter.ts`:

```bash
tsc greeter.ts
```

---

### Interfaces

```typescript
interface Person {
    firstName: string;
    lastName: string;
}

function greeter(person: Person) {
    return "Hello, " + person.firstName + " " + person.lastName;
}

var user = { firstName: "Jane", lastName: "User" };

document.body.innerHTML = greeter(user);
```

---

### Classes

```typescript
class Student {
    fullName: string;
    constructor(public firstName, public middleInitial, public lastName) {
        this.fullName = firstName + " " + middleInitial + " " + lastName;
    }
}

interface Person {
    firstName: string;
    lastName: string;
}

function greeter(person : Person) {
    return "Hello, " + person.firstName + " " + person.lastName;
}

var user = new Student("Jane", "M.", "User");

document.body.innerHTML = greeter(user);
```

---
