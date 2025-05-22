<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>JavaScript Identifier Rules</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 2rem;
    }
    code {
      background-color: #f4f4f4;
      padding: 2px 6px;
      border-radius: 4px;
    }
    pre {
      background-color: #f9f9f9;
      padding: 1rem;
      border-left: 5px solid #ccc;
      overflow-x: auto;
    }
    h2 {
      color: #007acc;
    }
    .warning {
      color: #e67e22;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <h1>JavaScript Identifier Rules</h1>

  <h2>✅ Valid Identifier Rules (Syntax Rules)</h2>
  <ul>
    <li>Can contain:
      <ul>
        <li>Letters (<code>A–Z</code>, <code>a–z</code>)</li>
        <li>Digits (<code>0–9</code>)</li>
        <li>Underscores (<code>_</code>)</li>
        <li>Dollar signs (<code>$</code>)</li>
      </ul>
    </li>
    <li>Cannot start with a digit</li>
  </ul>

  <pre><code>let 1abc = 10; // ❌ Invalid
let abc1 = 10; // ✅ Valid</code></pre>

  <ul>
    <li>Can start with a letter, <code>_</code>, or <code>$</code></li>
  </ul>

  <pre><code>let _name = "John"; // ✅
let $value = 42;    // ✅</code></pre>

  <ul>
    <li>Cannot be a reserved word or keyword (e.g., <code>let</code>, <code>if</code>, <code>class</code>)</li>
  </ul>

  <pre><code>let let = 5; // ❌ Invalid</code></pre>

  <ul>
    <li>Case-sensitive</li>
  </ul>

  <pre><code>let name = "Alice";
let Name = "Bob";
console.log(name); // "Alice"</code></pre>

  <ul>
    <li>Can use Unicode characters (including emojis, accented letters, etc.)</li>
  </ul>

  <pre><code>let café = "coffee";  // ✅ Valid
let 😊 = "happy";      // ✅ Valid (though not recommended)</code></pre>

  <h2 class="warning">⚠️ Best Practices (Naming Conventions)</h2>

  <h3>Use camelCase for variables and functions</h3>
  <pre><code>let userName = "John";
function getUserInfo() {}</code></pre>

  <h3>Use PascalCase for class names</h3>
  <pre><code>class UserAccount {}</code></pre>

  <h3>Avoid starting names with <code>_</code> unless for private-like members (by convention)</h3>
  <pre><code>let _internalValue = 100;</code></pre>

  <h3>Avoid using <code>$</code> unless working with jQuery or similar libraries</h3>
  <pre><code>let $button = document.querySelector("button");</code></pre>

  <h3>Choose meaningful names</h3>
  <pre><code>// Bad
let x = 10;

// Good
let userAge = 10;</code></pre>

</body>
</html>
