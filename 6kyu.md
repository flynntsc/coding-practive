
## 6 kyu


> [Tribonacci Sequence](https://www.codewars.com/kata/556deca17c58da83c00002db) 斐波纳契数列（HINT: push、slice）- Good

```
[1,1,1,3,5,9,17,31,...]
[0,0,1,1,2,4,7,13,24,...]
```

> [Unique In Order](https://www.codewars.com/kata/54e6533c92449cc251001667) 去除连续重复值（HINT: filter）- Clever

```
uniqueInOrder('AAAABBBCCDAABBB') == ['A', 'B', 'C', 'D', 'A', 'B']
uniqueInOrder('ABBCcAD')         == ['A', 'B', 'C', 'c', 'A', 'D']
uniqueInOrder([1,2,2,3,3])       == [1,2,3]
```

> [Your order, please](https://www.codewars.com/kata/55c45be3b2079eccff00010f) 按内含数字排序字符串（Hint：regex） - Good

```
function order(words){
	// "is2 Thi1s T4est 3a"
	// return "Thi1s is2 3a T4est"
}
```

> [Find the divisors!
](https://www.codewars.com/kata/544aed4c4a30184e960010f4) 列出可整除的数字（Hint: /2） - Clever

```
divisors(12); //should return [2,3,4,6]
divisors(25); //should return [5]
divisors(13); //should return "13 is prime"
```

> [Create Phone Number](https://www.codewars.com/kata/525f50e3b73515a6db000b83) 生成电话号码（Hint: for、replace）

```
createPhoneNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 0]) // => returns "(123) 456-7890"
```

> [Evil Autocorrect Prank](https://www.codewars.com/kata/538ae2eb7a4ba8c99b000439) 替换指定字符串（Hint: replace、/b）- Good


> [Function iteration](https://www.codewars.com/kata/54b679eaac3d54e6ca0008c9) 函数迭代（Hint: for）- Good

```
getDouble(3) => 6
getDouble(6) => 12

var createIterator = ???

var doubleIterator = createIterator(getDouble, 2); // This means, it runs *getDouble* twice
doubleIterator(3) => 12
```

> [Once](https://www.codewars.com/kata/5307ff5b588fe6d7000000a5) 只执行一次的函数（Hint: return）- Good

```
logOnce = once(console.log)
logOnce("foo") // -> "foo"
logOnce("bar") // -> no effect
```

> [Function Composition](https://www.codewars.com/kata/5421c6a2dda52688f6000af8) 函数合成（Hint: FP、closure）- Clever

```
f3 = compose( f1 f2 )
   Is equivalent to...
f3(a) = f1( f2( a ) )

compose(f , g)(x)
=> f( g( x ) )
```

> [Unary function chainer](https://www.codewars.com/kata/54ca3e777120b56cb6000710) 链式调用函数（Hint: FP、closure、reduce）- Good

```
chained([a,b,c,d])(input)
// =>
d(c(b(a(input))))
```

> [Palindrome for your Dome](https://www.codewars.com/kata/53046ceefe87e4905e00072a) 过滤反转字符串（Hint: regex、replace、reduce）- Clever

```
"Amore, Roma" => valid
"A man, a plan, a canal: Panama" => valid
"No 'x' in 'Nixon'" => valid
"Abba Zabba, you're my only friend" => invalid
```

> [Decode the Morse code](https://www.codewars.com/kata/54b724efac3d5402db00065e) 解码摩尔斯（Hint: Array、join、regex）

```
decodeMorse('.... . -.--   .--- ..- -.. .')
//should return "HEY JUDE"
```

> [IQ Test](https://www.codewars.com/kata/iq-test) 筛选与其他不同奇偶数字的位置（Hint: map、reduce）- Clever

```js
iqTest("2 4 7 8 10") => 3 // Third number is odd, while the rest of the numbers are even

iqTest("1 2 1 1") => 2 // Second number is even, while the rest of the numbers are odd
```

> [Find the odd int](https://www.codewars.com/kata/find-the-odd-int) 找出那个唯一的奇数个数的数值（Hint:\^,reduce）- Clever

```js
findOd([1,3,1]) // 3
```

> [https://www.codewars.com/kata/find-the-parity-outlier](https://www.codewars.com/kata/find-the-parity-outlier) 找出唯一的一个奇/偶数（Hint:filter）- Clever

```js
[2, 4, 0, 100, 4, 11, 2602, 36]

Should return: 11

[160, 3, 1719, 19, 11, 13, -21]

Should return: 160
```

> [Equal Sides Of An Array](https://www.codewars.com/kata/equal-sides-of-an-array) 对等切数组的位置（Hint:slice,reduce）- Clever

```js
findEvenIndex([1,2,3,4,3,2,1]) // 3
findEvenIndex([1,100,50,-51,1,1]) // 1
findEvenIndex([1,2,3,4,5,6]) // -1
findEvenIndex([20,10,30,10,10,15,35]) // 3
```

> [Stop gninnipS My sdroW!](https://www.codewars.com/kata/stop-gninnips-my-sdrow) 指定字符串中的单词反序（Hint: Regex,replace）- Clever

```js
spinWords( "Hey fellow warriors" ) => returns "Hey wollef sroirraw" 
spinWords( "This is a test") => returns "This is a test" 
spinWords( "This is another test" )=> returns "This is rehtona test"
```

