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

>[Merged String Checker](https://www.codewars.com/kata/merged-string-checker/javascript) 判读str是否由str1和str2组合（Hint：Recursion）- Clever

```
'codewars' is a merge from 'cdw' and 'oears':

    s:  c o d e w a r s   = codewars
part1:  c   d   w         = cdw
part2:    o   e   a r s   = oears
```

>[Weight for weight](https://www.codewars.com/kata/weight-for-weight/javascript) 数值之和以及字符串值的排序（Hint: localeCompare）- Good

```
56 65 74 100 99 68 86 180 90" ordered by numbers weights becomes: "100 180 90 56 65 74 68 86 99"

orderWeight("2000 10003 1234000 44444444 9999 11 11 22 123") // "11 11 2000 10003 22 123 1234000 44444444 9999"
```

> [Coding with Squared Strings](https://www.codewars.com/kata/coding-with-squared-strings/javascript) 正方形字符串的编译反编译运用（Hint:regexp、reduce、map）- Clever

```
t = "I.was.going.fishing.that.morning.at.ten.o'clock"

code(t) -> "c.nhsoI\nltiahi.\noentinw\ncng.nga\nk..mg.s\n\voao.f.\n\v'trtig"

decode(code(t)) == "I.was.going.fishing.that.morning.at.ten.o'clock"
```

>[Maximum subarray sum](https://www.codewars.com/kata/maximum-subarray-sum/javascript) 求子数组的最大之和（Hint: Math.max、.min）- Clever

```
maxSequence([-2, 1, -3, 4, -1, 2, 1, -5, 4])
// should be 6: [4, -1, 2, 1]
```

>[Number of trailing zeros of N!](https://www.codewars.com/kata/number-of-trailing-zeros-of-n/javascript) 数据递增相乘结果有几个零结尾（Hint:for、Recursion） - Clever

`末尾零均来源于2*5再来计算`

```
zeros(12) = 2 # 1 * 2 * 3 .. 12 = 479001600 
that has 2 trailing zeros 4790016(00)

zeros(30) // 7
zeros(100) // 24
zeros(100000) // 24999
```

>[Is my friend cheating?](https://www.codewars.com/kata/is-my-friend-cheating/javascript) 有无满足a*b = sum(n)-a-b的两个数（Hint:for）- Clever

```
removNb(26) should return [(15, 21), (21, 15)]

// sum(n) = 1 + 2 + 3 + ... + n-2 + n-1 + n
// a <= n && b <= n
// a * b = sum(n) - a - b
```

>[Did I Finish my Sudoku?](https://www.codewars.com/kata/did-i-finish-my-sudoku) 判断是否已完成九宫格（Hint:Array、双for）- Clever

![九宫格](http://upload.wikimedia.org/wikipedia/commons/thumb/3/31/Sudoku-by-L2G-20050714_solution.svg/364px-Sudoku-by-L2G-20050714_solution.svg.png)

```

```

>[Gap in Primes](https://www.codewars.com/kata/gap-in-primes/) 求素数区间内相邻的数（Hint:for）- Good

`有时间复杂度要求，除素数判断外，尽可能一个循环计算`

```
gap(2, 100, 110) // [101, 103]
gap(4, 100, 110) // [103, 107]
gap(6, 100, 110) // null
gap(8, 300, 400) // [359, 367]
gap(10, 300, 400) // [337, 347]
```

>[Product of consecutive Fib numbers](https://www.codewars.com/kata/product-of-consecutive-fib-numbers) 求一个数值是否为斐波那契数列相邻两个数之积（Hint: while）- Good

`简单的循环即可，而无需依靠数组`

```
productFib(714) # should return [21, 34, true], 
                # since F(8) = 21, F(9) = 34 and 714 = 21 * 34

productFib(800) # should return [34, 55, false], 
                # since F(8) = 21, F(9) = 34, F(10) = 55 and 21 * 34 < 800 < 34 * 55
```

>[Simple Pig Latin](https://www.codewars.com/kata/simple-pig-latin/) 替换字符串每个单词首字母移末尾（Hint:Array、map、reduce、Regexp）- Clever

`很简单但利用正则相当clever`

```
// Pig = ig + P + ay
pigIt('Pig latin is cool'); // igPay atinlay siay oolcay
```

>[Human Readable Time](https://www.codewars.com/kata/human-readable-time) 格式化秒数为时分秒（Hint:/、%、slice）- Good

`秒分直接计算可得，无需再相减`

```
HH = hours, padded to 2 digits, range: 00 - 99
MM = minutes, padded to 2 digits, range: 00 - 59
SS = seconds, padded to 2 digits, range: 00 - 59
```

>[What's a Perfect Power anyway?](https://www.codewars.com/kata/whats-a-perfect-power-anyway/javascript) 判断数值是否能被整数求根（Hint:for、Math）- Clever

`Math.pow(5,3) === 125`

but(216,343...)

`Math.pow(125,1/3) !== 5 === 4.999999999999999`

```
isPP(4) // [2,2]
isPP(9) // [3,2]
isPP(5) // null
```

>[Primes in numbers](https://www.codewars.com/kata/primes-in-numbers/javascript) 求数值的积数（Hint:for、while）- Good

```
Example: n = 86240 should return "(2**5)(5)(7**2)(11)"
```

>[Best travel](https://www.codewars.com/kata/best-travel/javascript) n个数值中挑出其中m个之和最合适值（Hint: Recursion、for）- Clever

```
ls = [50, 55, 57, 58, 60] // 5选3排列
all = [50,55,57],[50,55,58],[50,55,60],[50,57,58],[50,57,60],[50,58,60],[55,57,58],[55,57,60],[55,58,60],[57,58,60]
all-sum = [162, 163, 165, 165, 167, 168, 170, 172, 173, 175]
choose_best_sum(163, 3, ts) -> 163
```

>[Scramblies](https://www.codewars.com/kata/scramblies/javascript) 判断后一个字符串是否能被前一个完全排列起来（Hint:for、reduce、every）- Clever

```js
str1 is 'rkqodlw' and str2 is 'world' the output should return true.
str1 is 'cedewaraaossoqqyt' and str2 is 'codewars' should return true.
str1 is 'katas' and str2 is 'steak' should return false.
```
