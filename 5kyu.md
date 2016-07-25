## 5 kyu

- [Wrapped Function](https://www.codewars.com/kata/511ed4593ba69cba1a000002) 包裹函数（HINT: bind）- Good

```
Function.prototype.wrap = ???

function speak(name){
   return "Hello " + name;
}

speak = speak.wrap(function(original, yourName, myName){
   greeting = original(yourName);
   return greeting + ", my name is " + myName;
})

var greeting = speak("Mary", "Kate");
```

- [Greed is Good](https://www.codewars.com/kata/5270d0d18625160ada0000e4) 累计计分 （HINT: Array、forEach、reduce）- Clever
- [Write out numbers](https://www.codewars.com/kata/52724507b149fa120600031d) 数值转单词（HINT: Array、Math.floor、%、iteration）- Good

```
number2words(0) = 'zero'
number2words(99) = "ninety-nine"
number2words(100) = "one hundred"
number2words(1002) = "one thousand two"
number2words(888888) = "eight hundred eighty-eight thousand eight hundred eighty-eight"
```

- [Concatenating functions](https://www.codewars.com/kata/527176c487961e5900000106) 连接函数pipe（HINT: FP、bind or =>）- Clever

```
Function.prototype.pipe = ???

var addOne = function(e) { return e + 1 };

var square = function(e) { return e * e };

var result = [1,2,3,4,5].map(addOne.pipe(square)) //-> [4,9,16,25,36]
```

- [Calculating with Functions](https://www.codewars.com/kata/525f3eda17c7cd9f9e000b39) 加减乘除函数（Hint: FP）- Good

```
seven(times(five())); // must return 35
four(plus(nine())); // must return 13
eight(minus(three())); // must return 5
six(dividedBy(two())); // must return 3
```

- [A Chain adding function](https://www.codewars.com/kata/539a0e4d85e3425cb0000a88) 链式加法函数（Hint: FP、Currying、valueOf）- Good

```
add(1)(2); // returns 3
add(1)(2)(3); // 6
add(1)(2)(3)(4); // 10
add(1)(2)(3)(4)(5); // 15

add(1) // 1
var addTwo = add(2);
addTwo // 2
addTwo + 5 // 7
addTwo(3) // 5
addTwo(3)(5) // 10
```
