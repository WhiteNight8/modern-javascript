## F.prototype

如果F.prtotype是一个对象,那么new操作符会使用它为新对象设置[[Prototype]]

设置Rabbit.prototype=animal的字面意思是,当创建了一个new Rabbit时,把它的[[Prototype]]赋值animal

prototype是一个水平箭头,表示一个常规属性,[[Prototype]]是垂直的,表示rabbit继承animal

F.prototype仅用在new F时

### 默认的F.prototype,构造器属性

每个函数都有prototype属性,即使我们没有提供

默认的prototype时一个只有属性constructor的对象,属性constructor指向函数自身

### 总结

- F.prototype属性在new F被调用时为新对象的[[Protype]]属性
- F.prototype的值要么是一个对象要么就是null,其他值不起作用
- prototype属性仅在设置了一个构造函数,并通过new调用时才具有这种特殊影响

