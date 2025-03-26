# JavaScript String Methods 🌟

This document provides an overview of key JavaScript string methods with explanations and examples.

##  `at()`
Returns the character at a given index. Supports negative indexing.

**Syntax:**
```javascript
string.at(index);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "JavaScript";
console.log(str.at(0));  // Output: 'J'
console.log(str.at(-1)); // Output: 't' (last character)
```

</details>

---

##  `charAt()`
Returns the character at a specific index.

**Syntax:**
```javascript
string.charAt(index);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "Hello World";
console.log(str.charAt(0)); // Output: 'H'
console.log(str.charAt(6)); // Output: 'W'
```

</details>

---

##  `charCodeAt()`
Returns the Unicode (ASCII) value of the character at a specific index.

**Syntax:**
```javascript
string.charCodeAt(index);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let text = "ABC";
console.log(text.charCodeAt(0)); // Output: 65 (Unicode of 'A')
console.log(text.charCodeAt(1)); // Output: 66 (Unicode of 'B')
```

</details>

---

##  `codePointAt()`
Returns the Unicode code point of a character at a specified index. Useful for emojis or special symbols.

**Syntax:**
```javascript
string.codePointAt(index);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let emoji = "💖";
console.log(emoji.codePointAt(0)); // Output: 128150
```

</details>

---

##  `concat()`
Joins two or more strings together.

**Syntax:**
```javascript
string1.concat(string2, string3, ...);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let firstName = "John";
let lastName = "Doe";
let fullName = firstName.concat(" ", lastName);
console.log(fullName); // Output: "John Doe"
```

</details>

---

### 📌 **Key Differences Between Methods**
| Method | Purpose | Supports Negative Index? |
|--------|---------|-------------------------|
| `at()` | Returns character at index | ✅ Yes |
| `charAt()` | Returns character at index | ❌ No |
| `charCodeAt()` | Returns Unicode value | ❌ No |
| `codePointAt()` | Returns Unicode code point | ❌ No |
| `concat()` | Joins multiple strings | N/A |

---


##  `endsWith()`
Checks if a string ends with a specified substring.

**Syntax:**
```javascript
string.endsWith(searchString, length);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "Hello World";
console.log(str.endsWith("World")); // Output: true
console.log(str.endsWith("Hello")); // Output: false
```

</details>

---

##  `includes()`
Determines whether a string contains a specified substring.

**Syntax:**
```javascript
string.includes(searchString, position);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "JavaScript is awesome";
console.log(str.includes("JavaScript")); // Output: true
console.log(str.includes("Python")); // Output: false
```

</details>

---

##  `indexOf()`
Returns the first occurrence index of a specified substring, or -1 if not found.

**Syntax:**
```javascript
string.indexOf(searchValue, fromIndex);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "JavaScript is fun";
console.log(str.indexOf("is")); // Output: 11
console.log(str.indexOf("Python")); // Output: -1
```

</details>

---

##  `isWellFormed()`
Checks if a string contains valid Unicode characters.

**Syntax:**
```javascript
string.isWellFormed();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let validStr = "Hello";
console.log(validStr.isWellFormed()); // Output: true
```

</details>

---

##  `lastIndexOf()`
Returns the last occurrence index of a specified substring, or -1 if not found.

**Syntax:**
```javascript
string.lastIndexOf(searchValue, fromIndex);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "JavaScript JavaScript";
console.log(str.lastIndexOf("JavaScript")); // Output: 11
```

</details>
...

## `localeCompare()`
Compares two strings in the current locale.

**Syntax:**
```javascript
string1.localeCompare(string2);
```

<details>
  <summary>Click to see examples</summary>

```javascript
console.log("apple".localeCompare("banana")); // Output: -1
console.log("grape".localeCompare("grape")); // Output: 0
console.log("zebra".localeCompare("ant")); // Output: 1
```

</details>

---

## `match()`
Retrieves the result of matching a string against a regular expression.

**Syntax:**
```javascript
string.match(regexp);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let text = "I love JavaScript!";
console.log(text.match(/love/)); // Output: ["love", index: 2, input: "I love JavaScript!"]
console.log(text.match(/o/g)); // Output: ["o", "o"]
```

</details>

---

## `matchAll()`
Returns an iterator of all matched results using a regular expression.

**Syntax:**
```javascript
string.matchAll(regexp);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "test1 test2 test3";
let regex = /test(\d)/g;

for (let match of str.matchAll(regex)) {
    console.log(match);
}
```

</details>

---

## `normalize()`
Normalizes a Unicode string.

**Syntax:**
```javascript
string.normalize([form]);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "ç"; // 'c' with cedilla
console.log(str.normalize("NFC"));
```

</details>

---

## `padEnd()`
Pads the string with another string until the desired length is reached.

**Syntax:**
```javascript
string.padEnd(targetLength, padString);
```

<details>
  <summary>Click to see examples</summary>

```javascript
console.log("123".padEnd(5, "0")); // Output: "12300"
```

</details>

---

## `padStart()`
Pads the string from the beginning until the desired length is reached.

**Syntax:**
```javascript
string.padStart(targetLength, padString);
```

<details>
  <summary>Click to see examples</summary>

```javascript
console.log("123".padStart(5, "0")); // Output: "00123"
```

</details>

---

## `repeat()`
Repeats the string a specified number of times.

**Syntax:**
```javascript
string.repeat(count);
```

<details>
  <summary>Click to see examples</summary>

```javascript
console.log("Hello ".repeat(3)); // Output: "Hello Hello Hello "
```

</details>

---

## `replace()`
Replaces a substring or pattern in a string.

**Syntax:**
```javascript
string.replace(searchValue, newValue);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let text = "I love JavaScript";
console.log(text.replace("JavaScript", "Python")); // Output: "I love Python"
```

</details>

---

## `replaceAll()`
Replaces all occurrences of a substring.

**Syntax:**
```javascript
string.replaceAll(searchValue, newValue);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let text = "Hello world, world!";
console.log(text.replaceAll("world", "everyone")); // Output: "Hello everyone, everyone!"
```

</details>

---

## `search()`
Searches for a match using a regular expression and returns the index of the match.

**Syntax:**
```javascript
string.search(regexp);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let text = "Find the word JavaScript in this sentence.";
console.log(text.search(/JavaScript/)); // Output: 13
```

</details>

---



## JavaScript String Methods (Part 3) 🌟

This document continues with more JavaScript string methods, providing explanations and examples.

---

##  `slice()`
Extracts a section of a string and returns it as a new string without modifying the original.

**Syntax:**
```javascript
string.slice(startIndex, endIndex);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "Hello, World!";
console.log(str.slice(0, 5)); // Output: "Hello"
console.log(str.slice(-6));  // Output: "World!"
```

</details>

---

##  `split()`
Splits a string into an array based on a specified separator.

**Syntax:**
```javascript
string.split(separator, limit);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "apple,banana,grape";
console.log(str.split(",")); // Output: ["apple", "banana", "grape"]
console.log(str.split("", 3)); // Output: ["a", "p", "p"]
```

</details>

---

##  `startsWith()`
Checks if a string starts with a specified substring.

**Syntax:**
```javascript
string.startsWith(searchString, position);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "Hello, World!";
console.log(str.startsWith("Hello")); // Output: true
console.log(str.startsWith("World", 7)); // Output: true
```

</details>

---

##  `substring()`
Extracts part of a string between two indices.

**Syntax:**
```javascript
string.substring(startIndex, endIndex);
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "JavaScript";
console.log(str.substring(0, 4)); // Output: "Java"
console.log(str.substring(4)); // Output: "Script"
```

</details>

---

##  `toLocaleLowerCase()`
Converts a string to lowercase based on locale-specific rules.

**Syntax:**
```javascript
string.toLocaleLowerCase();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "İSTANBUL";
console.log(str.toLocaleLowerCase("tr-TR")); // Output: "istanbul"
```

</details>

---

##  `toLocaleUpperCase()`
Converts a string to uppercase based on locale-specific rules.

**Syntax:**
```javascript
string.toLocaleUpperCase();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "istanbul";
console.log(str.toLocaleUpperCase("tr-TR")); // Output: "İSTANBUL"
```

</details>

---

##  `toLowerCase()`
Converts a string to lowercase.

**Syntax:**
```javascript
string.toLowerCase();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "HELLO WORLD";
console.log(str.toLowerCase()); // Output: "hello world"
```

</details>

---

##  `toString()`
Returns the string representation of an object.

**Syntax:**
```javascript
value.toString();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let num = 123;
console.log(num.toString()); // Output: "123"

let bool = true;
console.log(bool.toString()); // Output: "true"
```

</details>

---

##  `toUpperCase()`
Converts a string to uppercase.

**Syntax:**
```javascript
string.toUpperCase();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "hello world";
console.log(str.toUpperCase()); // Output: "HELLO WORLD"
```

</details>

---

##  `toWellFormed()`
Checks if a string is well-formed Unicode.

**Syntax:**
```javascript
string.toWellFormed();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "Hello";
console.log(str.toWellFormed()); // Output: true
```

</details>

---

### 📌 **Summary Table**
| Method | Purpose |
|--------|---------|
| `slice()` | Extracts part of a string |
| `split()` | Splits a string into an array |
| `startsWith()` | Checks if string starts with substring |
| `substring()` | Extracts substring between two indices |
| `toLocaleLowerCase()` | Converts to lowercase (locale-aware) |
| `toLocaleUpperCase()` | Converts to uppercase (locale-aware) |
| `toLowerCase()` | Converts to lowercase |
| `toString()` | Converts value to string |
| `toUpperCase()` | Converts to uppercase |
| `toWellFormed()` | Checks Unicode well-formedness |

---


###  `trim()`
Removes whitespace from both ends of a string.

**Syntax:**
```javascript
string.trim();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "   Hello World!   ";
console.log(str.trim()); // Output: "Hello World!"
```

</details>

---

###  `trimEnd()`
Removes whitespace from the end of a string.

**Syntax:**
```javascript
string.trimEnd();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "   Hello World!   ";
console.log(str.trimEnd()); // Output: "   Hello World!"
```

</details>

---

###  `trimStart()`
Removes whitespace from the beginning of a string.

**Syntax:**
```javascript
string.trimStart();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "   Hello World!   ";
console.log(str.trimStart()); // Output: "Hello World!   "
```

</details>

---

###  `valueOf()`
Returns the primitive value of a string object.

**Syntax:**
```javascript
string.valueOf();
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = new String("Hello");
console.log(str.valueOf()); // Output: "Hello"
```

</details>

---

###  `Symbol.iterator`
Allows iteration over the characters of a string.

**Syntax:**
```javascript
string[Symbol.iterator];
```

<details>
  <summary>Click to see examples</summary>

```javascript
let str = "Hello";
let iterator = str[Symbol.iterator]();
console.log(iterator.next().value); // Output: "H"
console.log(iterator.next().value); // Output: "e"
```

</details>

---

### 📢 **How to Use This README**
- Click the dropdown arrows to expand and see examples.
- Copy-paste the code snippets to test in your JavaScript console.

---

### 🚀 **Contributions**
Feel free to contribute by adding more examples or explanations!



