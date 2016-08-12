## 4 kyu


- [Undo/Redo](https://www.codewars.com/kata/531489f2bb244a5b9f00077e) 撤销/重复操作（Hint: Array、stack）- Hard

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
- [Default Arguments](https://www.codewars.com/kata/52605419be184942d400003d) 默认函数（Hint: function、reg、match）- Hard

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

- [Dependency Injection](https://www.codewars.com/kata/5302d655be2a91068b0001fb) 依赖注射（Hint: reg、toString、apply、bind）- Hard

- [Next bigger number with the same digits](https://www.codewars.com/kata/55983863da40caa2c900004e) 下一个更大数值大小的队列（Hint:for、split、+1）- Clever

```
nextBigger(12)==21
nextBigger(513)==531
nextBigger(2017)==2071
```
