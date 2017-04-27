## 4 kyu


> [Undo/Redo](https://www.codewars.com/kata/531489f2bb244a5b9f00077e) 撤销/重复操作（Hint: Array、stack）- Hard

```
function undoRedo(object) {
	return {
		set: function(key, value) {},
		get: function(key) {},
		del: function(key) {},
		undo: function() {},
		redo: function() {}
	};
}
```
> [Default Arguments](https://www.codewars.com/kata/52605419be184942d400003d) 默认函数（Hint: function、reg、match）- Hard

```
function add(a,b) { return a+b;};

var add_ = defaultArguments(add,{b:9});
add_(10); // returns 19
add_(10,7); // returns 17
add_(); // returns NaN

add_ = defaultArguments(add_,{b:3, a:2});
add_(10); // returns 13 now
add_(); // returns 5

add_ = defaultArguments(add_,{c:3}); // doesn't do anything, since c isn't an argument
add_(10); // returns NaN
add_(10,10); // returns 20
```

> [Dependency Injection](https://www.codewars.com/kata/5302d655be2a91068b0001fb) 依赖注射（Hint: reg、toString、apply、bind）- Hard

> [Next bigger number with the same digits](https://www.codewars.com/kata/55983863da40caa2c900004e) 下一个更大数值大小的队列（Hint:for、split、+1）- Clever

```
nextBigger(12)==21
nextBigger(513)==531
nextBigger(2017)==2071
```

>[Remove Zeros](https://www.codewars.com/kata/remove-zeros/train/javascript) 不借助数组或对象方法将零排最后（Hint:for、i < l的情况i++，l++总次数不变）- Good

```
[7, 2, 3, 0, 4, 6, 0, 0, 13, 0, 78, 0, 0, 19, 14]

is transformed into

[7, 2, 3, 4, 6, 13, 78, 19, 14, 0, 0, 0, 0, 0, 0]
```

>[Recover a secret string from random triplets](https://www.codewars.com/kata/recover-a-secret-string-from-random-triplets/javascript) 从一个数组组合还原出单词（Hint: Recursion、for...of）- Clever

`所有数组中均在第一个必然是单词第一个，以此递归`

```
const secret1 = 'whatisup'
const triplets1 = [
  ['t', 'u', 'p'],
  ['w', 'h', 'i'],
  ['t', 's', 'u'],
  ['a', 't', 's'],
  ['h', 'a', 'p'],
  ['t', 'i', 's'],
  ['w', 'h', 's']
]

recoverSecret(triplets1) // 结果 secret1
```
>[Snail](https://www.codewars.com/kata/snail/javascript) 按不同的顺序拆解二维数组（Hint: for、Array、.pop、.shift、push、reverse）- Clever

`4个方向依次操作一遍作为循环`

```
array = [[1,2,3],
         [4,5,6],
         [7,8,9]]
snail(array) #=> [1,2,3,6,9,8,7,4,5]

array = [[1,2,3],
         [8,9,4],
         [7,6,5]]
snail(array) #=> [1,2,3,4,5,6,7,8,9]
```

![Snail图片事例](http://www.haan.lu/files/2513/8347/2456/snail.png)


>[Valid Braces](https://www.codewars.com/kata/valid-braces) 验证左右括号完全对应（Hint:Regular、while、replace）- Clever

```
validBraces( "(){}[]" ) => returns true 
validBraces( "(}" ) => returns false 
validBraces( "[(])" ) => returns false 
validBraces( "([{}])" ) => returns true
```

>[Roman Numerals Encoder](https://www.codewars.com/kata/roman-numerals-encoder) 罗马数字编译器（Hint:Array、Object、for、while）- Good

```
Symbol    Value
I          1
V          5
X          10
L          50
C          100
D          500
M          1,000

solution(1) // 'I'
solution(4) // 'IV'
solution(1000) // 'M'
solution(1990) // 'MCMXC'
solution(2007) // 'MMVII'
```

>[Reverse polish notation calculator](https://www.codewars.com/kata/reverse-polish-notation-calculator) 逆波兰表示法编译器（Hint:Array、Regexp、switch）- Clever

```
// 操作符前两数字优先计算
5 1 2 + 4 * + 3 - 等同于 5 + ((1 + 2) * 4) - 3
```

>[Human readable duration format](https://www.codewars.com/kata/human-readable-duration-format/) 将秒数格式化为人类易读模式（Hint: object、for...in、array、replace）- Clever

`直接计算也可，只是有更clever的方法`

```
  formatDuration(0)     //  return "now"   
  formatDuration(62)    // returns "1 minute and 2 seconds"
  formatDuration(3662)  // returns "1 hour, 1 minute and 2 seconds"
```

[Square into Squares. Protect trees!](https://www.codewars.com/kata/square-into-squares-protect-trees) 一个数平方是否等于其他不重复的数平方之和（Hint: Recursion）- Clever

`结果[x1 ... xk]，基本上xk都将是n-1`

`Skill Skill Skill: 将运算直接放在函数参数中；return fn(a1) || fn(a2)深度递归`

```
// 11² = 121 = 1 + 4 + 16 + 100 = 1² + 2² + 4² + 10²
// [2,6,9]虽也符合条件，但9<10，所以取较大值
decompose(11) // [1,2,4,10]
```

>[Sum Strings as Numbers](https://www.codewars.com/kata/sum-strings-as-numbers) 计算两个字符串的数值之和（Hint:for、Array、reverse）- Good

```
sumStrings('1','2') // => '3'
sumStrings('712569312664357328695151392','8100824045303269669937') // => '712577413488402631964821329'
```
