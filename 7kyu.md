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
