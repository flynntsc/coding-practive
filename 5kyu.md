## 5 kyu

- [Wrapped Function](https://www.codewars.com/kata/511ed4593ba69cba1a000002) 包裹函数（HINT: bind）- Good

```
Function.prototype.wrap = ???

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
