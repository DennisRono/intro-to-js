# Introduction to JavaScript: Beginner Introduction to JavaScript (All you need to Know)

JavaScript files have the file extension `.js`

## Keywords in JavaScript

Keywords are reserved words that have special meanings and are used to perform various operations within js
Keywords include:- `await`, `break`, `case`, `catch`, `class`, `const`, `continue`, `debugger`, `default`, `delete`, `do`, `else`, `enum`, `export`, `extends`, `false`, `finally`, `for`, `function`, `if`, `import`, `in`, `instanceof`, `new`, `null`, `return`, `super`, `switch`, `this`, `throw`, `true`, `try`, `typeof`, `var`, `void`, `while`, `with`, `yield` and many more.

## Variables

**[LAYMAN]**: Container for storing values

- `var`, `let`, or `const`
  Rules when declaring variables in js
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

Basic, immutable data types that hold the actual values and not references.

# Operations

JavaScript supports a wide variety of operations that can be performed on different data types. These operations can be arithmetic, comparison, logical, bitwise, assignment, and more.

### 1. Arithmetic Operations

These operations are used to perform mathematical calculations.

- **Addition (`+`)**: Adds two operands.
- **Subtraction (`-`)**: Subtracts the second operand from the first.
- **Multiplication (`*`)**: Multiplies two operands.
- **Division (`/`)**: Divides the first operand by the second.
- **Modulus (`%`)**: Returns the remainder of the division of the first operand by the second.
- **Exponentiation (`**`)\*\*: Raises the first operand to the power of the second operand.
- **Increment (`++`)**: Increases an operand by one.
- **Decrement (`--`)**: Decreases an operand by one.

### Example:

```javascript
let a = 10
let b = 5

console.log(a + b) // 15
console.log(a - b) // 5
console.log(a * b) // 50
console.log(a / b) // 2
console.log(a % b) // 0
console.log(a ** b) // 100000

a++
console.log(a) // 11

b--
console.log(b) // 4
```

### 2. Comparison Operations

These operations compare two operands and return a Boolean value (`true` or `false`).

- **Equal (`==`)**: Checks if two operands are equal (type conversion is performed).
- **Strict Equal (`===`)**: Checks if two operands are equal and of the same type.
- **Not Equal (`!=`)**: Checks if two operands are not equal (type conversion is performed).
- **Strict Not Equal (`!==`)**: Checks if two operands are not equal or not of the same type.
- **Greater Than (`>`)**: Checks if the first operand is greater than the second.
- **Less Than (`<`)**: Checks if the first operand is less than the second.
- **Greater Than or Equal (`>=`)**: Checks if the first operand is greater than or equal to the second.
- **Less Than or Equal (`<=`)**: Checks if the first operand is less than or equal to the second.

### Example:

```javascript
let x = 10
let y = 5

console.log(x == y) // false
console.log(x === y) // false
console.log(x != y) // true
console.log(x !== y) // true
console.log(x > y) // true
console.log(x < y) // false
console.log(x >= y) // true
console.log(x <= y) // false
```

### 3. Logical Operations

These operations are used to combine or invert Boolean values.

- **Logical AND (`&&`)**: Returns `true` if both operands are `true`.
- **Logical OR (`||`)**: Returns `true` if at least one operand is `true`.
- **Logical NOT (`!`)**: Inverts the Boolean value of the operand.

### Example:

```javascript
let a = true
let b = false

console.log(a && b) // false
console.log(a || b) // true
console.log(!a) // false
```

### 4. Bitwise Operations

These operations are performed on the binary representations of numbers.

- **Bitwise AND (`&`)**: Performs a binary AND operation.
- **Bitwise OR (`|`)**: Performs a binary OR operation.
- **Bitwise XOR (`^`)**: Performs a binary XOR operation.
- **Bitwise NOT (`~`)**: Inverts the bits of the operand.
- **Left Shift (`<<`)**: Shifts the bits of the first operand to the left by the number of positions specified by the second operand.
- **Right Shift (`>>`)**: Shifts the bits of the first operand to the right by the number of positions specified by the second operand.
- **Unsigned Right Shift (`>>>`)**: Shifts the bits of the first operand to the right by the number of positions specified by the second operand, filling the leftmost bits with zeros.

### Example:

```javascript
let a = 5 // 0101 in binary
let b = 3 // 0011 in binary

console.log(a & b) // 1 (0001 in binary)
console.log(a | b) // 7 (0111 in binary)
console.log(a ^ b) // 6 (0110 in binary)
console.log(~a) // -6 (inverts bits: 1010 in binary + 1 for two's complement)
console.log(a << 1) // 10 (1010 in binary)
console.log(a >> 1) // 2 (0010 in binary)
console.log(a >>> 1) // 2 (0010 in binary)
```

### 5. Assignment Operations

These operations assign values to variables.

- **Assignment (`=`)**: Assigns the right operand's value to the left operand.
- **Addition Assignment (`+=`)**: Adds the right operand to the left operand and assigns the result to the left operand.
- **Subtraction Assignment (`-=`)**: Subtracts the right operand from the left operand and assigns the result to the left operand.
- **Multiplication Assignment (`*=`)**: Multiplies the left operand by the right operand and assigns the result to the left operand.
- **Division Assignment (`/=`)**: Divides the left operand by the right operand and assigns the result to the left operand.
- **Modulus Assignment (`%=`)**: Takes the modulus of the left operand by the right operand and assigns the result to the left operand.
- **Exponentiation Assignment (`**=`)\*\*: Raises the left operand to the power of the right operand and assigns the result to the left operand.
- **Bitwise AND Assignment (`&=`)**: Performs a bitwise AND operation on the left operand and the right operand and assigns the result to the left operand.
- **Bitwise OR Assignment (`|=`)**: Performs a bitwise OR operation on the left operand and the right operand and assigns the result to the left operand.
- **Bitwise XOR Assignment (`^=`)**: Performs a bitwise XOR operation on the left operand and the right operand and assigns the result to the left operand.
- **Left Shift Assignment (`<<=`)**: Performs a left shift on the left operand by the number of positions specified by the right operand and assigns the result to the left operand.
- **Right Shift Assignment (`>>=`)**: Performs a right shift on the left operand by the number of positions specified by the right operand and assigns the result to the left operand.
- **Unsigned Right Shift Assignment (`>>>=`)**: Performs an unsigned right shift on the left operand by the number of positions specified by the right operand and assigns the result to the left operand.

### Example:

```javascript
let x = 10
x += 5 // x = x + 5
console.log(x) // 15

x -= 3 // x = x - 3
console.log(x) // 12

x *= 2 // x = x * 2
console.log(x) // 24

x /= 4 // x = x / 4
console.log(x) // 6

x %= 3 // x = x % 3
console.log(x) // 0

x **= 2 // x = x ** 2
console.log(x) // 0
```

### 6. String Operations

These operations are used to manipulate and combine strings.

- **Concatenation (`+`)**: Combines two or more strings.
- **Template Literals (`` ` ``)**: Embeds expressions within string literals using backticks.

### Example:

```javascript
let firstName = 'Dennis'
let lastName = 'Kibet'
let fullName = firstName + ' ' + lastName
console.log(fullName)

let age = 30
let greeting = `Hello, my name is ${firstName} ${lastName} and I am ${age} years old.`
console.log(greeting)
```

# Functions

functions are used to encapsulate a pieces of code that can be executed and reused.
functions are defined using the function keyword. They can be named or anonymous.

```javascript
function greet(name) {
  return `Hello, ${name}!`
}
console.log(greet('Kibet'))
```

Arrow functions provide a more concise syntax than normal functions, especially useful for short, single-expression functions.

```javascript
let add = (a, b) => {
  return a + b
}
console.log(add(2, 3))
```

# Conditional Statements

They are used to make decisions in code based on certain conditions.

## `if else` Statement

The `if` statement evaluates a condition inside parentheses. If the condition is true, the block of code inside the curly braces {} is executed. The `else` statement is used with an if statement to execute a block of code if the `if` condition evaluates to false.

```javascript
let temperature = 25

if (temperature > 30) {
  console.log("It's a hot day!")
} else {
  console.log("It's not very hot today.")
}
```

## Ternary Operator (`? :`)

The ternary operator provides a concise way to write simple if...else statements. It evaluates a condition and returns one value if true, and another value if false.

```javascript
let score = 75
let message = score >= 60 ? 'Pass' : 'Fail'

console.log(message)
```

## `switch` Statement

The `switch` statement is used to perform different actions based on different conditions. It evaluates an expression and matches the expression's value to a case clause, and executes the associated block of code.

```javascript
let day = 3
let dayName

switch (day) {
  case 1:
    dayName = 'Monday'
    break
  case 2:
    dayName = 'Tuesday'
    break
  case 3:
    dayName = 'Wednesday'
    break
  default:
    dayName = 'Unknown'
}

console.log(`Today is ${dayName}`)
```

# Loops

They are used to execute a block of code repeatedly until a specified condition evaluates to false. They provide a way to iterate over arrays, manipulate strings, and perform other repetitive tasks efficiently.

## `for` Loop

Use `for` when you know the number of iterations in advance.

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i)
}
```

## `while` Loop & `do...while` Loop

Use `while` and `do...while` when the number of iterations is determined by a condition.

```javascript
let count = 0
while (count < 3) {
  console.log(count)
  count++
}
```

```javascript
let i = 0
do {
  console.log(i)
  i++
} while (i < 3)
```

## `for...in` Loop

`for...in` is used to iterate over object properties.

```javascript
const person = {
  name: 'Dennis Kibet',
  age: 30,
  city: 'Nairobi',
}

for (let key in person) {
  console.log(`${key}: ${person[key]}`)
}
```

## `for...of` Loop

`for...of` is used to iterate over iterable objects like arrays and strings.

```javascript
const fruits = ['apple', 'banana', 'cherry']
for (let fruit of fruits) {
  console.log(fruit)
}
```

# Arrays and Objects

Arrays and objects are fundamental data structures in JavaScript, they are used for organizing and manipulating data.

## Arrays

Arrays are ordered collections of elements accessed by index, useful for lists of similar items.

**Creating Arrays:**

```javascript
// Array of numbers
let numbers = [1, 2, 3, 4, 5]

// Array of strings
let fruits = ['apple', 'banana', 'cherry']

// Mixed data types
let mixed = [1, 'apple', true, { name: 'Dennis' }]
```

**Accessing Array Elements:**

```javascript
console.log(fruits[0]) // Outputs: 'apple'
console.log(numbers.length) // Outputs: 5 (length of the array)
```

**Modifying Arrays:**

```javascript
fruits.push('orange') // Adds 'orange' to the end
fruits.pop() // Removes the last element ('cherry' in this case)
fruits[1] = 'pear' // Updates the element at index 1 to 'pear'
```

**Iterating Over Arrays:**

```javascript
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i])
}

// Using forEach
fruits.forEach(function (fruit) {
  console.log(fruit)
})
```

### Objects:

Objects are collections of key-value pairs, accessed by key, ideal for structured data with different properties.

**Creating Objects:**

```javascript
let person = {
  name: 'Kibet',
  age: 30,
  city: 'Nairobi',
}

// Accessing object properties
console.log(person.name) // Outputs: 'Alice'
console.log(person['age']) // Outputs: 30
```

**Adding and Modifying Properties:**

```javascript
person.email = 'kibet@example.com' // Adding a new property
person.age = 22 // Modifying an existing property
```

**Nested Objects:**

```javascript
let car = {
  make: 'Toyota',
  model: 'Camry',
  year: 2020,
  owner: {
    name: 'Dennis',
    age: 22,
  },
}

console.log(car.owner.name)
```

**Iterating Over Object Properties:**

```javascript
for (let key in person) {
  console.log(`${key}: ${person[key]}`)
}

// Using Object.keys()
Object.keys(person).forEach(function (key) {
  console.log(`${key}: ${person[key]}`)
})
```

# Events

Events are actions
Events in JavaScript allow you to respond to user actions and browser events, enhancing interactivity in your web applications.

# High Order Functions in JS

Higher-order functions in JavaScript accept or return functions, enabling flexible and concise coding by treating functions as values.

### .map()

```javascript
;[1, 2, 3, 4, 5].map((i) => {
  return i * 2
})
```

### .filter()

Filters elements of an array based on a condition and returns a new array with the filtered elements.

```javascript
const numbers = [1, 2, 3, 4, 5, 6]

const evenNumbers = numbers.filter((num) => num % 2 === 0)

console.log(evenNumbers)
```

### .reduce()

Reduces the elements of an array to a single value, applying a function to each element

```javascript
const numbers = [1, 2, 3, 4, 5]

const sum = numbers.reduce(
  (accumulator, currentValue) => accumulator + currentValue,
  0
)

console.log(sum)
```

### .forEach()

Executes a provided function once for each array element

```javascript
const fruits = ['apple', 'banana', 'cherry']

fruits.forEach((fruit) => {
  console.log(fruit)
})
```

### .find()

Returns the first element in the array that satisfies a provided testing function.

```javascript
const numbers = [10, 20, 30, 40, 50]

const foundNumber = numbers.find((num) => num > 25)

console.log(foundNumber)
```

### .some()

Checks if at least one element in the array satisfies a provided testing function

```javascript
const numbers = [1, 2, 3, 4, 5]

const hasEvenNumber = numbers.some((num) => num % 2 === 0)

console.log(hasEvenNumber)
```

### .every()

Checks if all elements in the array satisfy a provided testing function.

```javascript
const numbers = [2, 4, 6, 8, 10]

const allEvenNumbers = numbers.every((num) => num % 2 === 0)

console.log(allEvenNumbers)
```

### .sort()

Sorts the elements of an array in place and returns the sorted array.

```javascript
const fruits = ['banana', 'apple', 'cherry']

fruits.sort()

console.log(fruits)
```

### .concat()

Returns a new array comprised of the array on which it is called joined with other arrays and/or values.

```javascript
const array1 = [1, 2, 3]
const array2 = [4, 5, 6]

const newArray = array1.concat(array2)

console.log(newArray)
```

### .flatMap()

Maps each element using a mapping function, then flattens the result into a new array.

```javascript
const numbers = [1, 2, 3]

const doubledAndSquared = numbers.flatMap((num) => [num * 2, num * 2 + 1])

console.log(doubledAndSquared)
```

### setTimeout
