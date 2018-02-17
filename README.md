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