
# convertStringToNumber & convertNumberToString

https://codesandbox.io/s/convertstringtonumber-t72j2




# JavaScript 特殊的对象


- String Object

  string的length是不可写不删除

- Function Object

  - [[call]]  type 为 Function
  <!-- - [[Construct]] 可以 new， 返回对象 -->

- Array Object

  - [[length]] 难以模拟

  - [[DefineOwnProperty]] 

    - Property == length

      设置对象的length属性，根据length的变化对对象进行操作

      newLength > length 用空扩充数组
      newLength < length 截取数组


- Arguments Object

  [[callee]] 伪数组 caller

- Module Namespece

  [[Module]] 视为一个引入的模块

  [[Exports]] 视为一个导出的模块

- Object

  [[Get]] property被访问时调用  get

  [[Set]] property被赋值时调用 set

  [[GetPrototypeOf]] 获取对象原型

  [[SetPrototypeOf]] 设置对象原型

  [[GetOwnProperty]] 获取对象私有属性的描述列表

  [[HasProperty]] hasOwnProperty 私有属性判断

  [[IsExtensible]] 对象是否可扩展

  [[PreventExtensions]] 控制对象是否可以添加属性

  [[DefineOwnProperty]] 定义对象属性和性质

  [[Delete]] delete 操作符

  [[OwnPropertyKeys]] Object.keys() Object.entries() Object.values() 使用

  [[Call]] 能够调用call 

