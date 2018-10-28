#
  1.扩展运算符背后调用的是   遍历器接口（Symbol.iterator），如果一个对象没有部署这个接口，就无法转换。
  2.Array.from方法还支持  类似数组的对象   。所谓类似数组的对象，本质特征只有一点，即必须有length属性。

  set map array string arguments 都是“遍历器接口（Symbol.iterator）”
  原生具备 Iterator 接口的数据结构如下。

      Array
      Map
      Set
      String
      TypedArray
      函数的 arguments 对象
      NodeList 对象

  for...of循环可以使用的范围包括数组、Set 和 Map 结构、
  某些类似数组的对象（比如arguments对象、DOM NodeList 对象）、后文的 Generator 对象，以及字符串。


