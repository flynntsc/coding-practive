# Question

> [谈谈JS的观察者模式（自定义事件）](http://www.cnblogs.com/LuckyWinty/p/5796190.html) 设计模式、自定义事件、对象拷贝

```javascript
var Event = {
    // 通过on接口监听事件eventName
    // 如果事件eventName被触发，则执行callback回调函数
    on: function (eventName, callback) {
        // your code
    },
    // 触发事件 eventName
    emit: function (eventName, ...arr) {
        // your code
    }
}
```

```javascript
// 测试1
Event.on('test', function (result) {
    console.log(result);
});
Event.on('test', function () {
    console.log('test');
});
Event.emit('test', 'hello world'); // 输出 'hello world' 和 'test'

// 测试2
var person1 = {};
var person2 = {};
Object.assign(person1, Event);
Object.assign(person2, Event);
person1.on('call1', function () {
    console.log('person1');
});
person2.on('call2', function () {
    console.log('person2');
});
person1.emit('call1'); // 输出 'person1'
person1.emit('call2'); // 没有输出
person2.emit('call1'); // 没有输出
person2.emit('call2'); // 输出 'person2'
```

# Hint

设计模式、Copy、[Object.assign](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)

```javascript
var a = { x: 1, y: { z: 2 } }
var b = Object.assign({}, a) // 一级x不影响、y.z二级影响到复制源
var c = JSON.parse(JSON.stringify(a)) // 深拷贝不影响复制源

b.x = 0
console.log(a) // { x: 1, y: { z: 2 } } 不变
console.log(b) // { x: 0, y: { z: 2 } } x改变
console.log(c) // { x: 1, y: { z: 2 } } 不变

b.y.z = 9
console.log(a) // { x: 1, y: { z: 9 } } z跟着变 - 引用？
console.log(b) // { x: 0, y: { z: 9 } } z改变
console.log(c) // { x: 1, y: { z: 2 } } 不变

c.x = 3
console.log(a) // { x: 1, y: { z: 9 } } 不变
console.log(b) // { x: 0, y: { z: 9 } } 不变
console.log(c) // { x: 3, y: { z: 2 } } x改变

c.y.z = 7
console.log(a) // { x: 1, y: { z: 9 } } 不变
console.log(b) // { x: 0, y: { z: 9 } } 不变
console.log(c) // { x: 3, y: { z: 7 } } z改变
```

# Solution

```javascript
var Event = {
    // 通过on接口监听事件eventName
    // 如果事件eventName被触发，则执行callback回调函数
    on: function (eventName, callback) {
        if(!this.handles) {
            // this.handles = {}

            Object.defineProperty(this, 'handles', {
                value: {},
                enumerable: false,
                configurable: true,
                writeable: true,
            })
        }
        if(!this.handles[eventName]) {
            this.handles[eventName] = []
        }
        this.handles[eventName].push(callback)
    },
    // 触发事件 eventName
    emit: function (eventName, ...arr) {
        if(this.handles && this.handles[eventName]) {
            for(let i = 0; i < this.handles[eventName].length; i++) {
                this.handles[eventName][i](...arr)

                // this.handles[eventName][i].apply(this, arr)
            }
        }
    }
}
```
