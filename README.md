# Introduction to JavaScript

## Keywords in JavaScript

- eywords are reserved words that have special meanings and are used to perform various operations within js
- Keywords include:- `await`, `break`, `case`, `catch`, `class`, `const`, `continue`, `debugger`, `default`, `delete`, `do`, `else`, `enum`, `export`, `extends`, `false`, `finally`, `for`, `function`, `if`, `import`, `in`, `instanceof`, `new`, `null`, `return`, `super`, `switch`, `this`, `throw`, `true`, `try`, `typeof`, `var`, `void`, `while`, `with`, `yield` and many more.

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
let firstName = 'John'
let lastName = 'Doe'
let fullName = firstName + ' ' + lastName
console.log(fullName) // John Doe

let age = 30
let greeting = `Hello, my name is ${firstName} ${lastName} and I am ${age} years old.`
console.log(greeting) // Hello, my name is John Doe and I am 30 years old.
```

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
