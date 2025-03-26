# JavaScript String Methods 🌟

This document provides an overview of key JavaScript string methods with explanations and examples.

## 1️⃣ `at()`
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

## 2️⃣ `charAt()`
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

## 3️⃣ `charCodeAt()`
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

## 4️⃣ `codePointAt()`
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

## 5️⃣ `concat()`
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

## 📢 **How to Use This README**
- Click the dropdown arrows to expand and see examples.
- Copy-paste the code snippets to test in your JavaScript console.

---

### 🚀 **Contributions**
Feel free to contribute by adding more examples or explanations!

