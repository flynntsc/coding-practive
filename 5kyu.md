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

- [Function Cache](https://www.codewars.com/kata/525481903700c1a1ff0000e1) 缓存功能的函数（Hint: JSON.stringify、arguments、apply）- Good

```
var complexFunction = function(arg1, arg2) { /* complex calculation in here */ };
var cachedFunction = cache(complexFunction);

cachedFunction('foo', 'bar'); // complex function should be executed
cachedFunction('foo', 'bar'); // complex function should not be invoked again, instead the cached result should be returned
cachedFunction('foo', 'baz'); // should be executed, because the method wasn't invoked before with these arguments
```

- [Sum of Pairs](https://www.codewars.com/kata/54d81488b981293527000c8f) 数组中最早符合条件的一对数值（Hint: for、{}）- Clever

```
sum_pairs([11, 3, 7, 5], 10) // => [3,7]
sum_pairs([4, 3, 2, 3, 4], 6) // => [4,2]
sum_pairs([10, 5, 2, 3, 7, 5], 10) // => [3,7]
```

- [Twice linear](https://www.codewars.com/kata/5672682212c8ecf83e000050) 两次不同线性递增（Hint: for）

```
// y = 2 * x + 1 and z = 3 * x + 1
u = [1, 3, 4, 7, 9, 10, 13, 15, 19, 21, 22, 27, ...]
```

> [Directions Reduction](https://www.codewars.com/kata/directions-reduction) 东西南北的减少（Hint:reduce,Regex）- Clever

```js

dirReduc(["NORTH", "SOUTH", "SOUTH", "EAST", "WEST", "NORTH", "WEST"]) => ["WEST"]
dirReduc(["NORTH", "SOUTH", "SOUTH", "EAST", "WEST", "NORTH"]) => []

```

>[Merged String Checker](https://www.codewars.com/kata/merged-string-checker/javascript) 判读str是否由str1和str2组合（Hint：recursion）- Clever

```
'codewars' is a merge from 'cdw' and 'oears':

    s:  c o d e w a r s   = codewars
part1:  c   d   w         = cdw
part2:    o   e   a r s   = oears
```
