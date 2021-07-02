### 原型方法

proto不推荐使用的原因是指，js规范中规定，proto必须在浏览器环境下才能得到支持

现代方法有：

- Object.create(proto,[descriptors])利用给定的proto作为[[Prototype]]和可选的属性描述来创建一个空对象
- Object.getPrototypeOf(obj)返回对象obj的[[prototype]]
- Object.setPrototypeOf(obj,proto)将对象obj的[[Prototype]]设置为proto

### 原型简史

bug

