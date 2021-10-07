## Promise

1. 生产者代码:会做一些事,并且需要一些时间
2. 消费者代码:在生产者代码完成的第一时间能获得其工作成果
3. Promise:将生产者和消费者代码连接在一起的一个特殊的js对象

Promise对象的构造器

```js
let promise = new Promise(function(resolve, reject) {
  // executor（生产者代码，“歌手”）
});
```

传递给new Promise的函数被称为executor.当new Promsise被创建,executor会自动运行.它包含最终产出结果的生产者代码

当executor获取了结果,无论事早还是晚都没关系,它应该调用以下回调之一

- resolve(value)
- reject(error)





- 这儿的只用有一个结果或则一个error
- 以Error对象reject
- resolve/reject可以立即进行
- state和result都是内部的



### 消费者: then, catch,finally

#### then

#### catch

#### finally

这事执行清理的很好的处理程序

- finally处理程序没有参数
- finally处理程序将结果和error传递给下个处理程序

可以对settled的promise附加处理程序



| Promises             | Callbacks                                                    |
| -------------------- | ------------------------------------------------------------ |
| 允许按照自然顺序编码 | 在处理的地方必须有一个callback函数,在调用前必须直到如何处理结果 |
| 可多次调用.then      | 只能有一个回调                                               |

