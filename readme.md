## Intro to JavaScript & jQuery
### Girl Develop It, January 2015

#### Learning Resources
+ [Code School](https://www.codeschool.com/paths/javascript)
+ [Codecadamy](http://www.codecademy.com/en/tracks/javascript)
+ [Eloquent JavaScript](http://eloquentjavascript.net/)

#### Documentation
+ [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
+ [Can I Use](http://caniuse.com/)
+ [Stack Overflow](http://stackoverflow.com/)
+ [jQuery](http://api.jquery.com)

___

### Class One
[Slides](http://girldevelopit.github.io/gdi-core-javascript/class1.html) / [Code Snippets](https://github.com/girldevelopit/gdi-core-javascript/tree/master/class1)

+ Variables
  + Declare
  + Initialize
+ Basic Data Types
  + Strings: "Hello"
  + Numbers: 43110
  + undefined
  + null
+ Expressions
  + \+	Addition (Numbers and Strings)
  + \-	Subtraction
  + \*	Multiplication
  + /	Division
  + %	Modulus
  + ++	Increment
  + --	Decrement
+ 'if / else' statements
+ Comparisons
 + ===	Equality
 + !==	Inequality
 + \>	Greater than
 + \>=	Greater than or equal to
 + <	Less than
 + <=	Less than or equal to
+ Logic
  + &&	AND
  + ||	OR
  + !	NOT
+ Functions
  + arguments
  + returning values
  + scope

Snack Calculator - [Codepen](http://codepen.io/jeffreypierce/pen/jEmmKG)  
Function Scope - [Codepen](http://codepen.io/jeffreypierce/pen/pvPYEZ)

HTML to begin **Class Two** (index.html):
```
<html>
<head>
<title>My Site!</title>
</head>
<body>
<h2>My Awesome Calculator</h2>
<button onclick="calculate()">Calculate life time supply</button>
<script src = "javascript.js"></script>
</body>
</html>
```

JavaScript to begin **Class Two** (javascript.js):
```
var calculate = function() {
  var age = 26;
  var oldAge = 96;
  var perDay = 2;

  var days = (oldAge - age) * 356;
  var total = perDay * days;

  if(total > 40000) {
    alert("You will need " + total + " to last you until the ripe old age of " + oldAge + ". Wow! That's a lot!");
  } else {
    alert("You will need " + total + " to last you until the ripe old age of " + oldAge + ". You seem pretty reasonable");
  }
};
```
