## Symbol类型

对象的属性键只能是字符串或则Symbol类型

### Symbol

表示唯一标识

Symbol不会自动转换为字符串

需要用toString

### 隐藏属性

Symbol允许创建的对象的隐藏属性,代码的任何其他部分都不能意外访问或则重写这些属性

### 对象字面量中的Symbol

需要方括号

### symbol在for in 中会被跳过

Object.keys也会忽略他们

### 全局symbol

### 总结

symbol是唯一标识符的基本类型

