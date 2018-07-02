# Project Title
**Dive-Into-JavaScript**

# What are the java script data types

JavaScript supports three Primary, two Composite and two Special data types. Next, we list down the data types in each of the categories.

**Primary Data Types**
  1. String
  2. Number
  3. Boolean

**Composite Data Types**
  1. Object
  2. Array
  
**Special Data Types**
  1. Null
  2. Undefined

**Comparision operator == and ===**

```javascript
<script>
var x = '5'
document.write(x==5)

o/p : true
</script>
```

```javascript
<script>
var x = '5'
document.write(x===5)

o/p : false
</script>
```

Because in first example is matching only with the value 5. But in 2nd example it is matching with value first and then it is matching with the data type that is why giving output false for 2nd example.



**How to delete particular index element from array**

```javascript
<script>
var st = [1,2,3,4,5]
st.splice(2,1)
document.write(st)

o/p 1,2,4,5
</script>
```


**Arguments reserved keyword:**

arguments keyword is used to take the unlimited number of parameter from called function and assigned to itself.

**example**

```javascript
<script>
function sum() {
  for (i = 0, l = arguments.length; i < l; i++) {
    result += arguments[i];
  }
  return result;
}
document.write(sum(1,2,3));
</script>

o/p 6
```


**Associative Array in JavaScript**

Associative arrays are dynamic objects we can define in multiple ways:

```javascript
var arr = { "one": 1, "two": 2, "three": 3 };

document.write(arr["one"])

o/p 1
```

```javascript
var arr = new Object()
arr.name = "alok"
arr.designation = "full stack"
document.write(arr.name)

o/p alok
```



**closure in Javascript**

Closures are just a function with preserved data. In the below example1 we see that variable x is passed to the function myFunc. And same for example 2 we pass data from outerFunc() to innerFunc().


**example1:**


```javascript
<script>
var x = 10;
function myFunc() {
  var y = 5;
  return x+y
}

document.write(myFunc())
</script>
```


**example2:**

```javascript
<script>
function outerFunc(outer) {
   function innerFunc(inner) {
     return inner + outer
   }
   return innerFunc
}
var addToOuter = new outerFunc(10)
document.write(addToOuter(20))
</script>

o/p : 30

```


**What is Preprocessors of Javascript**

A library or framework etc that compiles to javascript is called preprocessors.


**JavaScript Properties**


Properties are the values associated with a JavaScript object, Like person.first.

**example**


```javascript
function employee(first, last) {
    this.first = first
    this.last] = last
}

var person = new employee("firstname", "lastname")

```


**Prototype**

1. JavaScript is a prototype-based language
2. All JavaScript objects inherit properties and methods from a prototype.


**JavaScript Hoisting**


Hoisting is JavaScript's standard default behavior of moving declarations to the top.

We can define the variaable or function as mention below but that is not js standard.

In JavaScript, a variable can be declared after it has been used.

In other words; a variable can be used before it has been declared.

``` javascript
x = 5; // Assign 5 to x
document.write(x)      // Display x in the element
var x;
```




  