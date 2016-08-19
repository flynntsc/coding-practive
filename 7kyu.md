## 7 kyu

- [Test Your Knowledge Of Function Scope](https://www.codewars.com/kata/test-your-knowledge-of-function-scope/javascript) 函数范围（Hint: function、return）- Good

```
add(3)(4)  // 7
add(12)(20) // 32
```

- [The Span Function](https://www.codewars.com/kata/the-span-function/solutions) 跨度函数（Hint: for） - Good

```
function isEven (x) {
  return Math.abs(x) % 2 === 0;
}

var arr = [2,4,6,1,8,10];

// This is true
span(arr, isEven) === [[2,4,6],[1,8,10]]
```

- [Pair Zeros](https://www.codewars.com/kata/pair-zeros/solutions) 过滤数字0（Hint: filter）- Clever

```
pairZeros([0,0]) // [0]
pairZeros([0,0,0]) // [0,0]
pairZeros([1,0,1,0,2,0,0,3,0]) // [1,0,1,2,0,3,0]
```

- [Beginner Series #3 Sum of Numbers](https://www.codewars.com/kata/55f2b110f61eb01779000053) 数值区间求和（Hint: Math、/2）- Clever

```
Example: 
GetSum(1, 0) == 1   // 1 + 0 = 1
GetSum(1, 2) == 3   // 1 + 2 = 3
GetSum(0, 1) == 1   // 0 + 1 = 1
GetSum(1, 1) == 1   // 1 Since both are same
GetSum(-1, 0) == -1 // -1 + 0 = -1
GetSum(-1, 2) == 2  // -1 + 0 + 1 + 2 = 2
```

- [All, None & Any](https://www.codewars.com/kata/54589f3b52756d34d6000158) 数组扩展方法（Hint: Array、filter）- Clever

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
- [Isograms](https://www.codewars.com/kata/54ba84be607a92aa900000f1) 判断是否有重复字符（Hint: regex）- Clever

```
isIsogram( "Dermatoglyphics" ) == true
isIsogram( "aba" ) == false
isIsogram( "moOse" ) == false // -- ignore letter case
```

- [Credit Card Mask](https://www.codewars.com/kata/5412509bd436bd33920011bc) 信用卡格式（Hint: regex、replace）- Clever

```
maskify("4556364607935616") == "############5616"
maskify(     "64607935616") ==      "#######5616"
maskify(               "1") ==                "1"
maskify(                "") ==                 ""

// "What was the name of your first pet?"
maskify("Skippy")                                   == "##ippy"
maskify("Nananananananananananananananana Batman!") == "####################################man!"
```

- [254 shades of grey](https://www.codewars.com/kata/54d22119beeaaaf663000024) 灰色的颜色格式-16进制（Hint:Math.min、slice）- Clever

- [Jaden Casing Strings](https://www.codewars.com/kata/5390bac347d09b7da40006f6) 格式化文字大小写（Hint: string、charAt、slice）- Good

```
Not Jaden-Cased: "How can mirrors be real if our eyes aren't real"
Jaden-Cased:     "How Can Mirrors Be Real If Our Eyes Aren't Real"
```
- [Complementary DNA](https://www.codewars.com/kata/complementary-dna) 字符串字母替换（Hint: object、replace）- Clever

```
DNAStrand ("ATTGC") # return "TAACG"

DNAStrand ("GTAT") # return "CATA"
```
