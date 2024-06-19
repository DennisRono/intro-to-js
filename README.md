# Introduction to JavaScript

## Keywords in JavaScript

- eywords are reserved words that have special meanings and are used to perform various operations within js
- Keywords include:- `await`, `break`, `case`, `catch`, `class`, `const`, `continue`, `debugger`, `default`, `delete`, `do`, `else`, `enum`, `export`, `extends`, `false`, `finally`, `for`, `function`, `if`, `import`, `in`, `instanceof`, `new`, `null`, `return`, `super`, `switch`, `this`, `throw`, `true`, `try`, `typeof`, `var`, `void`, `while`, `with`, `yield`

## Variables

- **[LAYMAN]**: Container for storing values
  - `var`, `let`, or `const`
- Rules when declaring variables in js
  - Variable names can contain letters, digits, underscores (\_), and dollar signs ($).
  - Variable names must begin with a letter, underscore, or dollar sign.
  - Variable names are case-sensitive (myVar and myvar are different variables).
  - Reserved words cannot be used as variable names (e.g., var, function, let, etc.).

## Data Types

### Number

Numerical value

```javascript
let number = 42
```

### String

Represents any data inside quotation marks `""`

```javascript
let name = 'kibet'
```

### Boolean

Yes/no; 0/1 - true/false data type

```javascript
let isHappy = true
```

### Null

Empty value

```javascript
let nullEmptyValue = null
```

### Undefined

A variable that has been declared but not yet assigned a value.

```javascript
let unassignedValue
```

### Object

Key value pair value (blueprint info)

```javascript
let person = {
  firstName: 'Dennis',
  lastName: 'Kibet',
  age: 21,
}
```

### Array

Data type for storing lists

```javascript
let fruits = ['Apple', 'Banana', 'Cherry']
```

### Symbol (ES6)

Represents a unique and immutable value that can be used as the key of an object property.

```javascript
let symbol1 = Symbol('description')
```

### BigInt (ES2020)

Allows you to represent whole numbers larger than 2^53 - 1, which is the largest number JavaScript can reliably represent with the Number type.

```javascript
let bigIntNumber = BigInt(1234567890123456789012345678901234567890)
let anotherBigInt = 1234567890123456789012345678901234567890n // Using the 'n' notation
```

### Primitive Data Types

- Basic, immutable data types that hold the actual values and not references.

# Operators

# Functions

# Conditional Statements

# Loops

# Arrays and Objects

# Events

# High Order Functions

### .map()

```javascript
;[1, 2, 3, 4, 5].map((i) => {
  return i * 2
})
```

### .filter()

### .reduce()

### .forEach()

### .find()

### .some()

### .every()

### .sort()

### .concat()

### .flatMap()
