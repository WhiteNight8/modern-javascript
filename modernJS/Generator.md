## Generator

常规函数只会返回一个单一值

而Genrator可以按需一个接着一个返回多个值

### Generator函数

next() 

- value:产出的值
- done: 如果generator函数已经执行完则为true,否则则为false



*最好跟函数在一起,表明函数类型



### Generator是可迭代的

for of 循环会忽略done为true时的value

### 总结

- Generator是通过function* f() {} 创建的
- 在generator内部存在yield操作
- 外部代码和generator可能会通过next/yield调用交换结果
- 