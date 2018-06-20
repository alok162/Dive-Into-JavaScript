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

**How to delete particular index element from array**

```javascript
<script>
var st = [1,2,3,4,5]
st.splice(2,1)
document.write(st)

o/p 1,2,4,5
</script>
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
  