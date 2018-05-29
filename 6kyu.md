
# 6 kyu


### [Tribonacci Sequence](https://www.codewars.com/kata/556deca17c58da83c00002db) 斐波纳契数列（HINT: push、slice）- Good

```js
[1,1,1,3,5,9,17,31,...]
[0,0,1,1,2,4,7,13,24,...]
```

### [Unique In Order](https://www.codewars.com/kata/54e6533c92449cc251001667) 去除连续重复值（HINT: filter）- Clever

```js
uniqueInOrder('AAAABBBCCDAABBB') == ['A', 'B', 'C', 'D', 'A', 'B']
uniqueInOrder('ABBCcAD')         == ['A', 'B', 'C', 'c', 'A', 'D']
uniqueInOrder([1,2,2,3,3])       == [1,2,3]
```

### [Your order, please](https://www.codewars.com/kata/55c45be3b2079eccff00010f) 按内含数字排序字符串（Hint：Regexp） - Good

```js
function order(words){
	// "is2 Thi1s T4est 3a"
	// return "Thi1s is2 3a T4est"
}
```

### [Find the divisors!
](https://www.codewars.com/kata/544aed4c4a30184e960010f4) 列出可整除的数字（Hint: /2） - Clever

```js
divisors(12); //should return [2,3,4,6]
divisors(25); //should return [5]
divisors(13); //should return "13 is prime"
```

### [Create Phone Number](https://www.codewars.com/kata/525f50e3b73515a6db000b83) 生成电话号码（Hint: for、replace）

```js
createPhoneNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 0]) // => returns "(123) 456-7890"
```

### [Evil Autocorrect Prank](https://www.codewars.com/kata/538ae2eb7a4ba8c99b000439) 替换指定字符串（Hint: replace、/b）- Good


### [Function iteration](https://www.codewars.com/kata/54b679eaac3d54e6ca0008c9) 函数迭代（Hint: for）- Good

```js
getDouble(3) => 6
getDouble(6) => 12

var createIterator = ???

var doubleIterator = createIterator(getDouble, 2); // This means, it runs *getDouble* twice
doubleIterator(3) => 12
```

### [Once](https://www.codewars.com/kata/5307ff5b588fe6d7000000a5) 只执行一次的函数（Hint: return）- Good

```js
logOnce = once(console.log)
logOnce("foo") // -> "foo"
logOnce("bar") // -> no effect
```

### [Function Composition](https://www.codewars.com/kata/5421c6a2dda52688f6000af8) 函数合成（Hint: FP、closure）- Clever

```js
f3 = compose( f1 f2 )
   Is equivalent to...
f3(a) = f1( f2( a ) )

compose(f , g)(x)
=> f( g( x ) )
```

### [Unary function chainer](https://www.codewars.com/kata/54ca3e777120b56cb6000710) 链式调用函数（Hint: FP、closure、reduce）- Good

```js
chained([a,b,c,d])(input)
// =>
d(c(b(a(input))))
```

### [Palindrome for your Dome](https://www.codewars.com/kata/53046ceefe87e4905e00072a) 过滤反转字符串（Hint: Regexp、replace、reduce）- Clever

```js
"Amore, Roma" => valid
"A man, a plan, a canal: Panama" => valid
"No 'x' in 'Nixon'" => valid
"Abba Zabba, you're my only friend" => invalid
```

### [Decode the Morse code](https://www.codewars.com/kata/54b724efac3d5402db00065e) 解码摩尔斯（Hint: Array、join、Regexp）

```js
decodeMorse('.... . -.--   .--- ..- -.. .')
//should return "HEY JUDE"
```

### [IQ Test](https://www.codewars.com/kata/iq-test) 筛选与其他不同奇偶数字的位置（Hint: map、reduce）- Clever

```js
iqTest("2 4 7 8 10") => 3 // Third number is odd, while the rest of the numbers are even

iqTest("1 2 1 1") => 2 // Second number is even, while the rest of the numbers are odd
```

### [Find the odd int](https://www.codewars.com/kata/find-the-odd-int) 找出那个唯一的奇数个数的数值（Hint:\^,reduce）- Clever

```js
findOd([1,3,1]) // 3
```

### [https://www.codewars.com/kata/find-the-parity-outlier](https://www.codewars.com/kata/find-the-parity-outlier) 找出唯一的一个奇/偶数（Hint:filter）- Clever

```js
[2, 4, 0, 100, 4, 11, 2602, 36]

Should return: 11

[160, 3, 1719, 19, 11, 13, -21]

Should return: 160
```

### [Equal Sides Of An Array](https://www.codewars.com/kata/equal-sides-of-an-array) 对等切数组的位置（Hint:slice,reduce）- Clever

```js
findEvenIndex([1,2,3,4,3,2,1]) // 3
findEvenIndex([1,100,50,-51,1,1]) // 1
findEvenIndex([1,2,3,4,5,6]) // -1
findEvenIndex([20,10,30,10,10,15,35]) // 3
```

### [Stop gninnipS My sdroW!](https://www.codewars.com/kata/stop-gninnips-my-sdrow) 指定字符串中的单词反序（Hint: Regexp,replace）- Clever

```js
spinWords( "Hey fellow warriors" ) => returns "Hey wollef sroirraw" 
spinWords( "This is a test") => returns "This is a test" 
spinWords( "This is another test" )=> returns "This is rehtona test"
```

### [Dubstep](https://www.codewars.com/kata/dubstep) 替换去除指定单词并拼接（Hint:split、filter）- Clever

```js
songDecoder("AWUBBWUBC") //"A B C"
songDecoder("AWUBWUBWUBBWUBWUBWUBC") //"A B C"
songDecoder("WUBAWUBBWUBCWUB") // "A B C"
```

### [Sum of Digits / Digital Root](https://www.codewars.com/kata/541c8630095125aba6000c00) 数值组合的不断求和（Hint:9 | reduce）- Clever

```js
digital_root(16)
=> 1 + 6
=> 7

digital_root(942)
=> 9 + 4 + 2
=> 15 ...
=> 1 + 5
=> 6

digital_root(132189)
=> 1 + 3 + 2 + 1 + 8 + 9
=> 24 ...
=> 2 + 4
=> 6

digital_root(493193)
=> 4 + 9 + 3 + 1 + 9 + 3
=> 29 ...
=> 2 + 9
=> 11 ...
=> 1 + 1
=> 2
```

### [Word a10n (abbreviation)](https://www.codewars.com/kata/word-a10n-abbreviation) 字符串替换（Hint: Regexp,replace）- Good

```js
abbreviate("elephant-rides are really fun!")
//          ^^^^^^^^*^^^^^*^^^*^^^^^^*^^^*
// words (^):   "elephant" "rides" "are" "really" "fun"
//                123456     123     1     1234     1
// ignore short words:               X              X

// abbreviate:    "e6t"     "r3s"  "are"  "r4y"   "fun"
// all non-word characters (*) remain in place
//                     "-"      " "    " "     " "     "!"
=== "e6t-r3s are r4y fun!"
```

### [Multiples of 3 and 5](https://www.codewars.com/kata/multiples-of-3-and-5)能整除3和5的数值之和（Hint:%）- Clever

```js
// <10 => 3+5+6+9 => 23
```

### [Duplicate Encoder](https://www.codewars.com/kata/54b42f9314d9229fd6000d9c) 字符串中重复/无重复的转化（Hint:String、Array）- Clever

```js
"din" => "((("

"recede" => "()()()"

"Success" => ")())())"

"(( @" => "))(("
```

### [ersistent Bugger.](https://www.codewars.com/kata/55bf01e5a717a0d57e0000ec) 数字不断相乘的次数（Hint:Loop、Recursion）- Clever

```js
persistence(39) === 3 // because 3*9 = 27, 2*7 = 14, 1*4=4 // and 4 has only one digit

 persistence(999) === 4 // because 9*9*9 = 729, 7*2*9 = 126, // 1*2*6 = 12, and finally 1*2 = 2

 persistence(4) === 0 // because 4 is already a one-digit number
```


### [Multi-tap Keypad Text Entry on an Old Mobile Phone](https://www.codewars.com/kata/54a2e93b22d236498400134b) 九宫格输入法按键次数计算（Hint:Array、Switch）- Clever

```

```

### [Give me Diamond](https://www.codewars.com/kata/give-me-diamond) 画个平行四边形/钻石(Hint：for、repeat、while) 从1个到n个\*来看、从n个到两边的1个\*来看- Clever

```js
diamond(5) // '  *\n ***\n*****\n ***\n  *\n'
// 效果如下
  *
 ***
*****
 ***
  *
```

### [Delete occurrences of an element if it occurs more than n times](https://www.codewars.com/kata/delete-occurrences-of-an-element-if-it-occurs-more-than-n-times) 过滤超过指定个数的数组（Hint:Object、filter）- Clever

```js
deleteNth([1, 1, 1, 1], 2) // return [1,1]

deleteNth([20, 37, 20, 21], 1) // return [20,37,21]
```

### [Format a string of names like 'Bart, Lisa & Maggie'](https://www.codewars.com/kata/53368a47e38700bd8300030d/solutions/javascript) 拼接数组中对象的属性（Hint:reduce、map、replace）- Clever

```js
list([ {name: 'Bart'}, {name: 'Lisa'}, {name: 'Maggie'} ])// returns 'Bart, Lisa & Maggie'list([ {name: 'Bart'}, {name: 'Lisa'} ])// returns 'Bart & Lisa'list([ {name: 'Bart'} ])// returns 'Bart'list([])// returns ''

```

### [Checking Groups](https://www.codewars.com/kata/checking-groups) 检测括号是否配对（Hint:Object）- Good

```js
// True
({})[[]()][{()}]

// False
{(})([][])
```

### [Regexp Basics - is it IPv4 address?](https://www.codewars.com/kata/regexp-basics-is-it-ipv4-address) 判断是否为IPv4地址（Hint:Regexp）- Clever

```js
"".ipv4Address() // false
"127.0.0.1".ipv4Address() // true
"0.0.0.0".ipv4Address() // true
"255.255.255.255".ipv4Address() // true
"10.20.30.40".ipv4Address() // true
"10.256.30.40".ipv4Address() // false
"10.20.030.40".ipv4Address() // false
"127.0.1".ipv4Address() // false
"127.0.0.0.1".ipv4Address() // false
"..255.255".ipv4Address() // false
"127.0.0.1\n".ipv4Address() // false
"\n127.0.0.1".ipv4Address() // false
" 127.0.0.1".ipv4Address() // false
"127.0.0.1 ".ipv4Address() // false
" 127.0.0.1 ".ipv4Address() // false
```

### [Rank Vector](https://www.codewars.com/kata/rank-vector) 排序位置标示（Hint:indexOf）- Good

```js
ranks([9,3,6,10]) = [2,4,3,1]

ranks([3,3,3,3,3,5,1]) = [2,2,2,2,2,1,7]
```

### ["this" is an other problem](https://www.codewars.com/kata/this-is-an-other-problem) 构造函数的值变化监听（Hint:Object.defineProperty）- Good

```js
var namedOne = new NamedOne("Naomi","Wang")

namedOne.firstName = "John"
namedOne.lastName = "Doe"
// ...then...
namedOne.fullName // -> "John Doe"

// -- And :
namedOne.fullName = "Bill Smith"
// ...then...
namedOne.firstName // -> "Bill"
namedOne.lastName  // -> "Smith"

// -- But :
namedOne.fullName = "Tom" // -> no : lastName missing
namedOne.fullName = "TomDonnovan" // -> no : no space between first & last names
namedOne.fullName // -> "Bill Smith" (unchanged)
```

### [Adjacent pairs in a string](https://www.codewars.com/kata/adjacent-pairs-in-a-string) 临近相同单词的个数（Hint:Regexp、match、\1）- Clever

```js
//returns 0
countAdjacentPairs('')

// returns 1
countAdjacentPairs('cat dog dog')

// returns 1 (The first pair has been matched, and will be ignored from then on).
countAdjacentPairs('dog dog dog')

// returns 2
countAdjacentPairs('cat cat dog dog cat')
```

### [Sequence generator](https://www.codewars.com/kata/sequence-generator) 序列迭代器（Hint:while、reduce）- Clever

```js
fib = sequenceGen(0, 1)
fib.next().value = 0 // first term (provided)
fib.next().value = 1 // second term (provided)
fib.next().value = 1 // third term (sum of first and second terms)
fib.next().value = 2 // fourth term (sum of second and third terms)
fib.next().value = 3 // fifth term (sum of third and fourth terms)
fib.next().value = 5 // sixth term (sum of fourth and fifth terms)
fib.next().value = 8 // seventh term (sum of fifth and sixth terms)

trib = sequenceGen(0,1,1)
trib.next().value = 0 // first term (provided)
trib.next().value = 1 // second term (provided)
trib.next().value = 1 // third term (provided)
trib.next().value = 2 // fourth term (sum of first, second and third terms)
trib.next().value = 4 // fifth term (sum of second, third and fourth terms)
trib.next().value = 7 // sixth term (sum of third, fourth and fifth terms)

lucas = sequenceGen(2,1);
arr = [];
for(i = 0;i < 10;i++){
  arr.push(lucas.next().value);
}
arr === [2, 1, 3, 4, 7, 11, 18, 29, 47, 76]
```

### [DNA Sequence Tester](https://www.codewars.com/kata/dna-sequence-tester) DNA序列配对测试（Hint:indexOf）- Clever

```js
seq1 = 'GTCTTAGTGTAGCTATGCATGC';  // NB up-down
seq2 = 'GCATGCATAGCTACACTACGAC';  // NB up-down

checkDNA (seq1, seq2);
// --> false

// Because there is a sequence mismatch at position 4:
// (seq1)    up-GTCTTAGTGTAGCTATGCATGC-down
//              ||| ||||||||||||||||||
// (seq2)  down-CAGCATCACATCGATACGTACG-up


seq1 = 'GCGCTGCTAGCTGATCGA';             // NB up-down
seq2 = 'ACGTACGATCGATCAGCTAGCAGCGCTAC';  // NB up-down

checkDNA (seq1, seq2);
// --> true

// Because one strand is entirely bonded by the other:
// (seq1)       up-GCGCTGCTAGCTGATCGA-down
//                 ||||||||||||||||||
// (seq2)  down-CATCGCGACGATCGACTAGCTAGCATGCA-up
```

### [Word Patterns](https://www.codewars.com/kata/word-patterns) 单词是否同规律排列（Hint:map、indexOf、every）- Clever

```js
wordPattern('abab', 'truck car truck car') === true
wordPattern('aaaa', 'dog dog dog dog') === true
wordPattern('abab', 'apple banana banana apple') === false
wordPattern('aaaa', 'cat cat dog cat') === false
```

### [知乎上问题](https://zhuanlan.zhihu.com/p/23981897) 判断 N 个布尔值是否全部相等（Hint:arr.indexOf） - Clever

```js
return arr.indexOf(!arr[0]) < 0
```

### [Multiples of 3 and 5 redux](https://www.codewars.com/kata/multiples-of-3-and-5-redux) 3或5的倍数之和（Hint: | 0）- Clever

```js
solution (10) // => 23 = 3 + 5 + 6 + 9
solution (20) // => 78 = 3 + 5 + 6 + 9 + 10 + 12 + 15 + 18
```

### [Calculate the function f(x) for a simple linear sequence (Easy)](http://www.codewars.com/kata/calculate-the-function-f-x-for-a-simple-linear-sequence-easy) 写出公式（Hint:三元符号）- Clever

```

```

### [String incrementer](https://www.codewars.com/kata/string-incrementer) 字符串加1（Hint:slice）- Clever

```
```

### [Are they the "same"?](https://www.codewars.com/kata/are-they-the-same/javascript) 判断两个数组是否相同（Hint：every、join）- Clever

```js
a = [121, 144, 19, 161, 19, 144, 19, 11] 
b = [11*11, 121*121, 144*144, 19*19, 161*161, 19*19, 144*144, 19*19]

a,b = []、null...

comp(a, b)
```

### [Bit Counting](https://www.codewars.com/kata/bit-counting/javascript) 计算数值二进制1的数量（Hint:>>=、toString）- Clever

```js
1234 => 10011010010 => 5 个 1
``` 

>[Moves in squared strings (II)](https://www.codewars.com/kata/moves-in-squared-strings-ii/javascript)字符串正方形颠倒旋转2（Hint:replace,Regexp）- Clever

```js
let s = "abcd\nefgh\nijkl\nmnop"
oper(rot, s) => "ponm\nlkji\nhgfe\ndcba"
oper(selfie_and_rot, s) => "abcd....\nefgh....\nijkl....\nmnop....\n....ponm\n....lkji\n....hgfe\n....dcba"
```

>[Moves in squared strings (III)](http://www.codewars.com/kata/moves-in-squared-strings-iii/javascript) 字符串正方形颠倒旋转3（Hint: map）- Clever

```js
let s = "abcd\nefgh\nijkl\nmnop"
oper(diag_1_sym, s) => "aeim\nbfjn\ncgko\ndhlp"
oper(rot_90_clock, s) => "miea\nnjfb\nokgc\nplhd"
oper(selfie_and_diag1, s) => "abcd|aeim\nefgh|bfjn\nijkl|cgko\nmnop|dhlp"
```
>[Password generator](https://www.codewars.com/kata/password-generator/javascript) 密码生成器（Hint:Math.random、题目可以更难一点）- Good

```js
6 - 20 characters long
contains at least one lowercase letter
contains at least one uppercase letter
contains at least one number
contains only alphanumeric characters (no special characters)
```

>[Simple Fun #170: Sum Groups
](https://www.codewars.com/kata/simple-fun-number-170-sum-groups/javascript) 过滤数组直到没有连续的奇、偶数（Hint:for、Recursion）- Clever

```js
[2, 1, 2, 2, 6, 5, 0, 2, 0, 5, 5, 7, 7, 4, 3, 3, 9]  -->
        2+2+6       0+2+0     5+5+7+7       3+3+9
[2, 1,   10,    5,    2,        24,     4,   15   ] -->
                             2+24+4
[2, 1,   10,    5,             30,           15   ]
The length of final array is 6
```

>[Cycle Detection: greedy algorithm](https://www.codewars.com/kata/cycle-detection-greedy-algorithm/javascript) 符合c=ax+b公式的数组求值（Hint:for、object键值的运用）- Clever

```js
cycle([2,3,4,2,3,4]) // [0,3]
cycle([1,2,3,4]) // []
```

>[Counting Duplicates](https://www.codewars.com/kata/counting-duplicates/javascript) 字符串中重复字的个数（Hint：sort、Regexp、\1、filter、lastIndexOf）- Clever 

```js
"abcde" -> 0 # no characters repeats more than once
"aabbcde" -> 2 # 'a' and 'b'
"aabbcdeB" -> 2 # 'a' and 'b'
"indivisibility" -> 1 # 'i'
"Indivisibilities" -> 2 # 'i' and 's'
"aa11" -> 2 # 'a' and '1'
```

>[Which are in?](https://www.codewars.com/kata/which-are-in/javascript) 数组2中字符串是否包含数组1中的字符串（Hint:Array、filter、some）- Clever

```js
a1 = ["arp", "live", "strong"]
a2 = ["lively", "alive", "harp", "sharp", "armstrong"]
returns ["arp", "live", "strong"]

a1 = ["tarp", "mice", "bull"]
a2 = ["lively", "alive", "harp", "sharp", "armstrong"]
returns []
```

>[Simple Encryption #1 - Alternating Split](https://www.codewars.com/kata/simple-encryption-number-1-alternating-split/javascript) 简单的加密与解密-交叉分离组合（Hint:Regexp、replace）- Clever

`除了遍历index判断，还可直接正则过滤`

```js
"This is a test!", 1 -> "hsi  etTi sats!"
"This is a test!", 2 -> "hsi  etTi sats!" -> "s eT ashi tist!"

function encrypt(text, n)
function decrypt(encryptedText, n)
```

>[Take a Number And Sum Its Digits Raised To The Consecutive Powers And ....¡Eureka!!](https://www.codewars.com/kata/5626b561280a42ecc50000d1/) 计算数字各位上累计求幂之和等于本身的数（Hint:while更简单、Math.pow的简写x**y）- Clever

`知道结果结合的情况下，可直接写出集合再直接判断即可，最省时省力`

```js
In effect: 89 = 8^1 + 9^2
The next number in having this property is 135.
See this property again: 135 = 1^1 + 3^2 + 5^3

sumDigPow(1, 10) == [1, 2, 3, 4, 5, 6, 7, 8, 9]

sumDigPow(1, 100) == [1, 2, 3, 4, 5, 6, 7, 8, 9, 89]

sumDigPow(90, 100) == []
```

>[Build Tower](https://www.codewars.com/kata/build-tower) 用数组表示一个金字塔（Hint:Array、Array.from、[...arr]、repeat）- Clever

```js
// 3 floors
[
  '  *  ', 
  ' *** ', 
  '*****'
]

6 floors
[
  '     *     ', 
  '    ***    ', 
  '   *****   ', 
  '  *******  ', 
  ' ********* ', 
  '***********'
]
```

>[Is a number prime?](https://www.codewars.com/kata/is-a-number-prime/javascript) 判断数值是否为素数（Hint:for、6n+-1、i * i <= num） - Clever

`代码最少方法、计算最少方法`

```js
isPrime(-2) === true
isPrime(0) === false
isPrime(1) === false
isPrime(2) === true
```
>[The Supermarket Queue](https://www.codewars.com/kata/the-supermarket-queue) 超市结账队列与窗口数的消耗时间计算（Hint: for、Math） - Clever

`以窗口为对象，计算各窗口消耗的时间，再求出最大值`

```js
queueTime([5,3,4], 1)
// should return 12
// because when n=1, the total time is just the sum of the times

queueTime([10,2,3,3], 2)
// should return 10
// because here n=2 and the 2nd, 3rd, and 4th people in the 
// queue finish before the 1st person has finished.

queueTime([2,3,10], 2)
// should return 12
```

>[Take a Ten Minute Walk](https://www.codewars.com/kata/take-a-ten-minute-walk) 东南西北走十步是否能回到原地（Hint:Object、Array、switch）- Clever

```
```

>[Find the missing letter](https://www.codewars.com/kata/find-the-missing-letter) 找出中间缺失的字母（Hint:charCodeAt、fromCharCode VS codePointAt、fromCodePoint = 后者ES6更完善）- Good

```js
['a','b','c','d','f'] -> 'e'
['O','Q','R','S'] -> 'P'
```
>[Triple trouble](https://www.codewars.com/kata/triple-trouble-1/) 连续数字是否再次出现（Hint:Regexp、for）- Clever

```js
tripledouble(451999277, 41177722899) == 1 // num1 has straight triple 999s and 
                                          // num2 has straight double 99s

tripledouble(1222345, 12345) == 0 // num1 has straight triple 2s but num2 has only a single 2

tripledouble(12345, 12345) == 0

tripledouble(666789, 12345667) == 1
```

>[Sort the odd](https://www.codewars.com/kata/sort-the-odd/javascript) 对数组中的奇数进行排序（Hint:filter、sort、map）- Clever

```js
sortArray([5, 3, 2, 8, 1, 4]) == [1, 3, 2, 8, 5, 4]
```

>[Playing with passphrases](https://www.codewars.com/kata/playing-with-passphrases/javascript) 简单的密码加密（Hint:replace、Regexp）- Clever

```js
your text: "BORN IN 2015!", shift 1

1 + 2 + 3 -> "CPSO JO 7984!"

4 "CpSo jO 7984!"

5 "!4897 Oj oSpC"
```

### [Simple Fun #259: Different Digits Number Search](https://www.codewars.com/kata/59113da398dcd456270000a8) 找出没重复数值的数（Hint:find、Regexp）- Clever

```js
For arr = [22, 111, 101, 124, 33, 30], the output should be 124

For arr = [1111, 404], the output should be -1
```

### [Simple Fun #256: Two Arrays Nth Element](https://www.codewars.com/kata/simple-fun-number-256-two-arrays-nth-element) 计算两个有序数组最小的第n个值（Hint:while、Math、Infinity）- Clever

`莫忘Infinity`

```js
twoArraysNthElement([1, 3, 4],[2, 6, 8],5) // 8
twoArraysNthElement([1, 3, 5],[2, 4],2) // 3
twoArraysNthElement([6,19,21,30,34,35,44,48],[3,4,5,9,14,16,25,32,36,37,41,53],11) // 32
```

### [Simple arithmetic progression](https://www.codewars.com/kata/simple-arithmetic-progression/javascript) 算出长度为3的数组组合相减值相等的数量（Hint: 多个for）- Clever

列出所有组合 or 直接计算数量 or 通过已得2个数值反推第3个是否存在

```js
[1, 2, 3, 5, 7, 9] ==> 5
// [1, 2, 3], [1, 3, 5], [1, 5, 9], [3, 5, 7], and [5, 7, 9]
```

### [RuplesJS #2: String Delete](https://www.codewars.com/kata/ruplesjs-number-2-string-delete/javascript) 扩展字符串的delete方法（Hint: typeof、reduce）- Good

参数（支持多参数）：字符串则全局删除；正则表达式则直接替换、其他如数值则无效无视

```js
"1: Are you enjoying this kata?".delete(/[^a-z ]/gi) -> " Are you enjoying this kata"
"1: Are you enjoying this kata?".delete("a", "?", [], /[0-9]/g) -> ": Are you enjoying this kt"
```
