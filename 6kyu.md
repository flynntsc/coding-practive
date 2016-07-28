
## 6 kyu


- [Tribonacci Sequence](https://www.codewars.com/kata/556deca17c58da83c00002db) 斐波纳契数列（HINT: push、slice）- Good

```
[1,1,1,3,5,9,17,31,...]
[0,0,1,1,2,4,7,13,24,...]
```

- [Unique In Order](https://www.codewars.com/kata/54e6533c92449cc251001667) 去除连续重复值（HINT: filter）- Clever

```
uniqueInOrder('AAAABBBCCDAABBB') == ['A', 'B', 'C', 'D', 'A', 'B']
uniqueInOrder('ABBCcAD')         == ['A', 'B', 'C', 'c', 'A', 'D']
uniqueInOrder([1,2,2,3,3])       == [1,2,3]
```

- [Your order, please](https://www.codewars.com/kata/55c45be3b2079eccff00010f) 按内含数字排序字符串（Hint：reg） - Good

```
function order(words){
	// "is2 Thi1s T4est 3a"
	// return "Thi1s is2 3a T4est"
}
```

- [Find the divisors!
](https://www.codewars.com/kata/544aed4c4a30184e960010f4) 列出可整除的数字（Hint: /2） - Clever

```
divisors(12); //should return [2,3,4,6]
divisors(25); //should return [5]
divisors(13); //should return "13 is prime"
```

- [Create Phone Number](https://www.codewars.com/kata/525f50e3b73515a6db000b83) 生成电话号码（Hint: for、replace）

```
createPhoneNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 0]) // => returns "(123) 456-7890"
```

- [Evil Autocorrect Prank](https://www.codewars.com/kata/538ae2eb7a4ba8c99b000439) 替换指定字符串（Hint: replace、/b）- Good


- [Function iteration](https://www.codewars.com/kata/54b679eaac3d54e6ca0008c9) 函数迭代（Hint: for）- Good

```
getDouble(3) => 6
getDouble(6) => 12

var createIterator = ???

var doubleIterator = createIterator(getDouble, 2); // This means, it runs *getDouble* twice
doubleIterator(3) => 12
```

- [Once](https://www.codewars.com/kata/5307ff5b588fe6d7000000a5) 只执行一次的函数（Hint: return）- Good

```
logOnce = once(console.log)
logOnce("foo") // -> "foo"
logOnce("bar") // -> no effect
```

- [Function Composition](https://www.codewars.com/kata/5421c6a2dda52688f6000af8) 函数合成（Hint: FP、closure）- Clever

```
f3 = compose( f1 f2 )
   Is equivalent to...
f3(a) = f1( f2( a ) )

compose(f , g)(x)
=> f( g( x ) )
```



