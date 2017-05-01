## 8 kyu

- [Double Char](https://www.codewars.com/kata/56b1f01c247c01db92000076) 重复字符串（Hint: replace）- Clever

```
doubleChar("String") ==> "SSttrriinngg"

doubleChar("Hello World") ==> "HHeelllloo  WWoorrlldd"

doubleChar("1234!_ ") ==> "11223344!!__  "
```

- [Sum of positive](https://www.codewars.com/kata/5715eaedb436cf5606000381) 数组求和（Hint:reduce） - Clever

```
[1,-4,7,12] => 1 + 7 + 12 = 20
```
> [Nth Root of a Number](https://www.codewars.com/kata/5520714decb43308ea000083) 求根（Hint:Math.pow）

```
root(4, 2);   // 2 (the square root of 4 is 2 , 2^2 = 4);
root(8, 3);   // 2 (the cube root of 8 is 2   , 2^3 = 8);
root(256, 4); // 4 (the 4th root of 256 is 4  , 4^4 = 256);
root(9, 2);   // 3 (the square root of 9 is 3 , 3^2 = 9)
```

> [Sum without highest and lowest number](https://www.codewars.com/kata/sum-without-highest-and-lowest-number/javascript) 计算除最小和最大值外之和（Hint：slice小细节）- Good

```
{ 6, 2, 1, 8, 10 } => 16
{ 1, 1, 11, 2, 3 } => 6
```
>[To square(root) or not to square(root)](https://www.codewars.com/kata/to-square-root-or-not-to-square-root/javascript) 过滤数组求平方根或平方（Hint:map、%1判断整数方法）- Clever

```
If the number has an integer square root, take this, otherwise square the number.

[4,3,9,7,2,1] -> [2,9,3,49,4,1]
```
>[Rock Paper Scissors!](https://www.codewars.com/kata/rock-paper-scissors/train/javascript) 算出石头剪刀布结果（Hint:Regexp、Object）- Clever

```
rps('scissors','paper') // Player 1 won!
rps('scissors','rock') // Player 2 won!
rps('paper','paper') // Draw!
```
>[Number of People in the Bus](https://www.codewars.com/kata/number-of-people-in-the-bus/javascript) 公交站数之和（Hint:reduce、参数写法）- Clever

```
number([[10,0],[3,5],[5,8]]) // 5
number([[3,0],[9,1],[4,10],[12,2],[6,1],[7,10]]) //17
```

>[Grasshopper - Summation](https://www.codewars.com/kata/grasshopper-summation/javascript) 简单的求和（Hint:数学定律）- Clever

```
summation(2) -> 3
1 + 2

summation(8) -> 36
1 + 2 + 3 + 4 + 5 + 6 + 7 + 8

eg:
1 + 2 + 3 + 4 + ... + n-3 + n-2 + n-1 + n
```

>[Fake Binary](https://www.codewars.com/kata/fake-binary/javascript) 转为只有01的字符串（Hint:array、join）- Clever

`x < 5 ? 0 : 1` VS `x / 5 | 0`

```
// 小于5 => 0, 不小于5 => 1
fakeBin('45385593107843568') // '01011110001100111'
```
