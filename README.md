# javascript-rev
review concepts

```
// What will the below code print out?
	.	"use strict";
	.	var a = 1;
	.	var b = {};
	.	function foo(x, y) {
	.	  x = 2;
	.	y.moo = 3;
	.	}
	.	 
	.	foo(a, b);
	.	console.log("a = " + a + "; b = " + JSON.stringify(b));
		 ```



```
     // What will the below code print out?
    var asimsVar = 3;
    asimVar = 1;
       console.log(asimVar)
```

```
```
// What will the below code print out?
	.	"use strict"; var asimsVar = 3; asimVar = 1; console.log(asimVar);
What does the below code print out?
if (undefined == null) {
console.log("Moo")
} else {
console.log("Zoo")
}

```

```
// What does the below code print out?
console.log(typeof(null));

// What does the below code print out?
if (undefined === null) {
console.log("Moo")
} else {
console.log("Zoo") 
}
```

```
// What will the below code print out?
console.log(NaN == “1");

```
```
// What happens when you execute the code below
a = 1;
```
```
// What does this print out?
console.log(typeof(null));
```
```
// What will the below code print out? 
"use strict";
var name = 'igloo';
var code = "var name = 'asim';"
eval(code)
console.log(name)
```
```
// What will this code print?
(function(){
var a = 3;
})();
console.log("a defined? " + (typeof a !== ‘undefined'));
```
```
// What will this code print?
// https://gist.github.com/jawache/7153e555fea2db73b952
console.log(moo);
var moo = function() {
console.log("loo");
};

```
```
// Consider the following code snippet:

for (var i = 0; i < 5; i++) {
  var btn = document.createElement('button');
  btn.appendChild(document.createTextNode('Button ' + i));
  btn.addEventListener('click', function () {
    console.log(i);
  });
  document.body.appendChild(btn);
}

// What gets logged to the console when the user clicks on “Button 4” and why?
```
```
// What will the following code output to the console?

console.log((function f(n){return ((n > 1) ? n * f(n-1) : n)})(4));

```
```

// Consider the code snippet below. 
//What will the console output be?

(function(x) {

return (function(y) {

console.log(x);

})(2)

})(1);

```
```
// https://gist.github.com/jawache/3cddd2b0a27f8ea6a460
// Consider the code snippet below. What will the console output?

function loo() {
  var goo = 1;
  moo();
}

function moo() {
  console.log(goo);
}

loo();

undefined

1
```

```
// What will be the output of first console.log in the code below?

var salary = "1000$";

(function () {

console.log("Original salary was " + salary);

var salary = "5000$";

console.log("My New Salary " + salary);

})();


Original salary was 5000$

Original salary was 1000$
```
```
// What would the below code print out?

function Device(kind) {
  this.kind =  kind;
  this.printKind = function () {
    console.log(this.kind)
  }
}


var product = new Device("music player");
product.printKind();
```
```
// What would the below code print out?

function Device(kind) {
  this.kind =  kind;
  this.printKind = function () {
    console.log(kind)
  }
}

var product = new Device("music player");
product.kind = "radio";
product.printKind();
```
```
// How would you create an instance of this pseudo-class using the constructor pattern?
function Device(kind) {
  this.kind =  kind;
}

var product = new Device("music player");
var product = Device("music player");
var product = Device.call("music player");
```
```
// What would the below code print out?

function Device(kind) {
  this.kind =  kind;
}

Device.prototype.printKind = function () {
  console.log(this.kind);
};

var product = new Device("music player");
product.printKind();
```
```
// We want AppleProduct to inherit from Device. Whats the best method of setting the kind property?

function Device(kind) {
  this.kind =  kind;
}

function AppleProduct(name, kind) {
  this.name = name;
}

//A)
function AppleProduct(name, kind) {
  this.name = name;
  this.kind = kind;
}

//B)
function AppleProduct(name, kind) {
  this.name = name;
  Device.call(this, kind);
}

//C)
function AppleProduct(name, kind) {
  this.name = name;
  Device(kind);
}

```


```

 What does the below code print out?
	.	"use strict";
	.	 
	.	var animal = {
	.	  kind: "Cow",
	.	  which: function () {
	.	    console.log(this.kind);
	.	  }
	.	};
	.	var animalFunc = animal.which;
	.	animalFunc();
```