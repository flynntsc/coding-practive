## 7 kyu

> [Test Your Knowledge Of Function Scope](https://www.codewars.com/kata/test-your-knowledge-of-function-scope/javascript) 函数范围（Hint: function、return）- Good

```
add(3)(4)  // 7
add(12)(20) // 32
```

> [The Span Function](https://www.codewars.com/kata/the-span-function/solutions) 跨度函数（Hint: for） - Good

```
function isEven (x) {
  return Math.abs(x) % 2 === 0;
}

var arr = [2,4,6,1,8,10];

// This is true
span(arr, isEven) === [[2,4,6],[1,8,10]]
```

> [Pair Zeros](https://www.codewars.com/kata/pair-zeros/solutions) 过滤数字0（Hint: filter）- Clever

```
pairZeros([0,0]) // [0]
pairZeros([0,0,0]) // [0,0]
pairZeros([1,0,1,0,2,0,0,3,0]) // [1,0,1,2,0,3,0]
```

> [Beginner Series #3 Sum of Numbers](https://www.codewars.com/kata/55f2b110f61eb01779000053) 数值区间求和（Hint: Math、/2）- Clever

```
Example: 
GetSum(1, 0) == 1   // 1 + 0 = 1
GetSum(1, 2) == 3   // 1 + 2 = 3
GetSum(0, 1) == 1   // 0 + 1 = 1
GetSum(1, 1) == 1   // 1 Since both are same
GetSum(-1, 0) == -1 // -1 + 0 = -1
GetSum(-1, 2) == 2  // -1 + 0 + 1 + 2 = 2
```

> [All, None & Any](https://www.codewars.com/kata/54589f3b52756d34d6000158) 数组扩展方法（Hint: Array、filter）- Clever

```
[1, 2, 3].all(isGreaterThanZero) => true
[-1, 0, 2].all(isGreaterThanZero) => false
[-1, 2, 3].none(isLessThanZero) => false
[-1, -2, -3].none(isGreaterThanZero) => true
[-1, 2, 3].any(isGreaterThanZero) => true
[-1, -2, -3].any(isGreaterThanZero) => false

function isGreaterThanZero (num) {
  return num > 0;
}
function isLessThanZero (num) {
  return num < 0;
}
```
> [Isograms](https://www.codewars.com/kata/54ba84be607a92aa900000f1) 判断是否有重复字符（Hint: regex）- Clever

```
isIsogram( "Dermatoglyphics" ) == true
isIsogram( "aba" ) == false
isIsogram( "moOse" ) == false // -- ignore letter case
```

> [Credit Card Mask](https://www.codewars.com/kata/5412509bd436bd33920011bc) 信用卡格式（Hint: regex、replace）- Clever

```
maskify("4556364607935616") == "############5616"
maskify(     "64607935616") ==      "#######5616"
maskify(               "1") ==                "1"
maskify(                "") ==                 ""

// "What was the name of your first pet?"
maskify("Skippy")                                   == "##ippy"
maskify("Nananananananananananananananana Batman!") == "####################################man!"
```

> [254 shades of grey](https://www.codewars.com/kata/54d22119beeaaaf663000024) 灰色的颜色格式-16进制（Hint:Math.min、slice）- Clever

> [Jaden Casing Strings](https://www.codewars.com/kata/5390bac347d09b7da40006f6) 格式化文字大小写（Hint: string、charAt、slice）- Good

```
Not Jaden-Cased: "How can mirrors be real if our eyes aren't real"
Jaden-Cased:     "How Can Mirrors Be Real If Our Eyes Aren't Real"
```
> [Complementary DNA](https://www.codewars.com/kata/complementary-dna) 对应DNA串-字符串字母替换（Hint: object、replace）- Clever

```
DNAStrand ("ATTGC") # return "TAACG"

DNAStrand ("GTAT") # return "CATA"
```

> [Descending Order](http://www.codewars.com/kata/descending-order/javascript) 递减顺序(Hint: sort、reverse) - Good

```
// reverse is better than sort((x,y)=>y-x)
Input: 145263 Output: 654321

Input: 1254859723 Output: 9875543221
```

> [Product of the main diagonal of a square matrix.](http://www.codewars.com/kata/product-of-the-main-diagonal-of-a-square-matrix) 数组对角乘法（Hint:reduce）- Clever

> [Highest and Lowest](http://www.codewars.com/kata/highest-and-lowest/javascript) 取最大值与最小值(Hint: Math、...) - Good

```
highAndLow("1 2 3 4 5"); // return "5 1"
highAndLow("1 2 -3 4 5"); // return "5 -3"
highAndLow("1 9 3 4 -5"); // return "9 -5"
```

> [Mumbling](http://www.codewars.com/kata/mumbling/javascript) 重复字符显示（Hint: map、Array、join）- Clever

```
accum("abcd");    // "A-Bb-Ccc-Dddd"
accum("RqaEzty"); // "R-Qq-Aaa-Eeee-Zzzzz-Tttttt-Yyyyyyy"
accum("cwAt");    // "C-Ww-Aaa-Tttt"
```

> [Regex validate PIN code](http://www.codewars.com/kata/regex-validate-pin-code/javascript) 正则PIN验证（Hint: regex）- Good

> [Vampire Numbers](https://www.codewars.com/kata/54d418bd099d650fa000032d) 数字相乘等于乘数组合（Hint: Array&String）- Good

```
6 * 21 = 126
# 6 and 21 would be valid 'fangs' for a vampire number as the 
# digits 6, 1, and 2 are present in both the product and multiplicands

10 * 11 = 110
# 110 is not a vampire number since there are three 1's in the
# multiplicands, but only two 1's in the product
```

> [Find the middle element](http://www.codewars.com/kata/find-the-middle-element) 找出中间大小的那个数（Hint: Array）

> [List to Array](https://www.codewars.com/kata/557dd2a061f099504a000088) next对象迭代为数组（Hint: Iterative）- Clever

```
{value: 1, next: {value: 2, next: {value: 3, next: null}}} => [1, 2, 3]
```

> [Sum of the first nth term of Series](https://www.codewars.com/kata/555eded1ad94b00403000071) 递增求和（Hint: for or recursive）- Clever

```
Series: 1 + 1/4 + 1/7 + 1/10 + 1/13 + 1/16 +...

SeriesSum(1) => 1 = "1"
SeriesSum(2) => 1 + 1/4 = "1.25"
SeriesSum(5) => 1 + 1/4 + 1/7 + 1/10 + 1/13 = "1.57"
```

> [Categorize New Member](https://www.codewars.com/kata/5502c9e7b3216ec63c0001aa) 判断是否符合条件（Hint: map）- Clever

```
[[18, 20],[45, 2],[61, 12],[37, 6],[21, 21],[78, 9]]
// =>
["Open", "Open", "Senior", "Open", "Open", "Senior"]
```

> [Flatten](https://www.codewars.com/kata/5250a89b1625e5decd000413) 数组降维度（Hint:concat）- Good

```
flatten([1,2,3]) // => [1,2,3]
flatten([[1,2,3],["a","b","c"],[1,2,3]])  // => [1,2,3,"a","b","c",1,2,3]
flatten([[[1,2,3]]]) // => [[1,2,3]]
```

> [Binary Calculator](https://www.codewars.com/kata/binary-calculator/javascript) 二进制计算（Hint:parseInt、toString）- Good

```
1 + 1 === 10
10 + 10 === 100
```

> [Linked Lists - Push & BuildOneTwoThree](https://www.codewars.com/kata/linked-lists-push-and-buildonetwothree)   （Hint:new、function）- Hard

```
var chained = null
chained = push(chained, 3)
chained = push(chained, 2)
chained = push(chained, 1)
push(chained, 8) === 8 -> 1 -> 2 -> 3 -> null
```
> [Complete The Pattern #2](https://www.codewars.com/kata/55733d3ef7c43f8b0700007c) 字符串拼接模式（Hint: for、String） - Clever

```
pattern(1)  => '1'
pattern(2) => "21\n2"
pattern(5) => "54321\n5432\n543\n54\n5"
```

> [Tug-o'-War](https://www.codewars.com/kata/tug-o-war) 两个数组大小比较结果（Hint: if、Array）- Clever

```
[[5,0,3,2,1], [1,6,8,2,9]]  // 11 < 26 ; "Team 2 wins!"
```

> [Invalid Input - Error Handling #1](https://www.codewars.com/kata/invalid-input-error-handling-number-1) 元音字母过滤计数（Hint: regex,replace）- Clever

```
Input: getCount('test')
Output: {vowels:1,consonants:3}

Input: getCount('tEst')
Output: {vowels:1,consonants:3}

Input getCount('    ')
Output: {vowels:0,consonants:0}

Input getCount()
Output: {vowels:0,consonants:0}
```

> [Find the capitals](https://www.codewars.com/kata/find-the-capitals-1) 字符串中大写的位置（Hint:Array、String） - Clever

```
Test.assertSimilar( capitals('CodEWaRs'), [0,3,4,6] )
```

> [SequenceSum](https://www.codewars.com/kata/sequencesum) 序列化排序（Hint: Array） - Clever

```
5 -> [0, 1, 3, 6, 10, 15]

-5 -> [0, -1, -3, -6, -10, -15]

7 -> [0, 1, 3, 6, 10, 15, 21, 28]
```

> [Collatz Conjecture Length](https://www.codewars.com/kata/collatz-conjecture-length) 考拉兹猜想个数计算（Hint: while）- Clever
