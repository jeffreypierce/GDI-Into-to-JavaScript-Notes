## Intro to JavaScript & jQuery
### Girl Develop It, January 2015

Teacher: **Jeffrey Pierce**  
[jeffrey@jeffreypierce.net](mailto: jeffrey@jeffreypierce.net)
, [@jeffrey_pierce](https://twitter.com/jeffrey_pierce)

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

### Class Two

##### Bonus Question!!!
You work for a hipster e-commerce website and your boss *needs* to know which items sold for over $40 in the last three days.

You do a query of your recent sales and get this array of objects:
```
var purchases = [
  {
    item: "Tote bag",
    timestamp: "Sat Jan 21 2015 09:12:31 GMT-0500 (EST)",
    amount: 45.99
  },
  {
    item: "Seitan",
    timestamp: "Sat Jan 22 2015 18:47:22 GMT-0500 (EST)",
    amount: 15.76
  },
  {
    item: "Bicycle",
    timestamp: "Sat Jan 21 2015 12:45:47 GMT-0500 (EST)",
    amount: 100.00
  },
  {
    item: "PBR",
    timestamp: "Sat Jan 17 2015 01:12:33 GMT-0500 (EST)",
    amount: 35.98
  },
  {
    item: "Sriracha",
    timestamp: "Sat Jan 14 2015 14:18:12 GMT-0500 (EST)",
    amount: 24.99
  },
  {
    item: "McSweeney's",
    timestamp: "Sat Jan 07 2015 11:11:11 GMT-0500 (EST)",
    amount: 78.90
  },
  {
    item: "Schlitz",
    timestamp: "Sat Jan 13 2015 13:45:12 GMT-0500 (EST)",
    amount: 22.87
  },
  {
    item: "Hoodie",
    timestamp: "Sat Jan 24 2015 05:14:22 GMT-0500 (EST)",
    amount: 50.00
  },
  {
    item: "Cardigan",
    timestamp: "Sat Jan 22 2015 13:33:32 GMT-0500 (EST)",
    amount: 45.67
  },
  {
    item: "Narwhal Heirloom",
    timestamp: "Sat Jan 21 2015 09:01:00 GMT-0500 (EST)",
    amount: 134.00
  }
];
```
With your new found JavaScript skills you decide to loop over this object and create a new array with the name of these specific items. And the day is saved!

*hint*
An easy way to compare dates is with the `.getTime()` method. It returns the number of milliseconds since January 1st 1970.

i.e. `var yesterday = new Date("Sat Jan 23 2015 09:01:00 GMT-0500 (EST)").getTime()`
