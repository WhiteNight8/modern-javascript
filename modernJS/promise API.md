## Promise API

在Promise类中,有5中方法静态方法

### Promise.all

```js
let promise = Promise.all([...promises...]);
```

当所有给定的promise都被settled时,新的Promise才会resolve.并且其结果数组将成为新的Promise的结果

**注意,结果中数组中元素的顺序跟其源promise中的顺序相同**



如果任意一个promise被reject,由promise.all返回的promise就会立即reject,并且带有的就是这个error

### Promise.allSettled

如果任意的promise reject,则Promise.all整个将会reject.

这个等待所有的promise都被settle



### Promise.race

等待第一个settled的promise并获取其结果

### Promise.resovle/reject

### 总结

Promise类5种静态方法

- Promise.all
- Promise.allSettled
- Promise.race
- Promise.resolve
- Promise.reject



## Promisification

