
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

## 5 kyu

- [Wrapped Function](https://www.codewars.com/kata/511ed4593ba69cba1a000002) 包裹函数（HINT: bind）- Good

```
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



