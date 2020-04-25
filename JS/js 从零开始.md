### 1. js数据类型
* 基本数据类型：Number, String, Boolean, Null, Undefined
* 引用数据类型：Array, Object, Function, Data

### 2. 数组方法
* 改变原数组：
  push：接受任意数量的参数，添加到数组末尾，返回新数组的长度
  pop：删除数组最后一项，返回删除的项
  shift：删除数组第一项，返回删除的项
  unshift：接受任意数量的参数，添加到数组头部，返回新数组的长度
  reverse：反转数组的顺序，并返回重新排序之后的数组
  sort：返回值为排序后的新数组
  splice：
    1. 删除：arr.splice(index, num)，返回删除元素组成的数组，参数有两个，第一个是起始位置，第二个是删除的项数
    2. 插入：arr.splice(index, num, item)，参数分别为 起始位置（ 数组下标） | 要删除的项数 | 要插入的元素， 返回删除掉的元素组成的数组
    3. 替换：arr.splice(index, num, item)，参数分别为 起始位置 | 要删除的项数 | 要插入的任意项数，返回删除掉的元素组成的数组

* 不改变原数组： 
  concat：合并数组，不传参，返回复制后的新数组；传递参数，返回合并后的数组
  slice: 截取数组，返回截取的元素组成的数组，参数有两个，开始位置和结束位置；若只给一个参数，则结束位置是数组的末尾。
  indexOf：查找元素，验证数组中是否含有某个元素，返回第一个匹配到的元素在数组中所在的位置，如果没有，则返回 -1
  lastIndexOf: 查找元素,从数组尾部开始查找，返回第一个匹配到的元素所在的位置，如果没有，则返回-1
  join: 给定一个连接符，连接所有数组元素组成一个字符串。


### 数组的迭代方法
* arr.forEach() 对数组中的每一项运行给定函数，这个方法没有返回值
* arr.every() 检查数组中的项是否满足某个条件，传入的函数对每一项都返回true,则返回true
* arr.some() 检查数组中的项是否满足某个条件，只要传入的函数对数组中某一项返回true,则返回true
* arr.filter() 将所有在过滤函数中返回 true 的数组元素放进一个新数组中并返回
* arr.map() 对数组中的每一项运行给定函数，返回每次函数调用的结果组成的新数组
* arr.reduce() 从左到右为每个数组元素执行一次回调函数，并把上次回调函数的返回值放在一个暂存器中传给下次回调函数，并返回最后一次回调函数的返回值。

tips: map、forEach里不可以使用continue、break ,每一项都会执行


### 判断数组的方式
* arr instanceof Array
* arr.constructor == Array
* arr.__proto__ == Array.prototype
* Object.prototype.toString.call(arr) == '[object Array]'
* Array.isArray(arr)

tips：不能用typeof arr来判断，因为该方式对数组和对象返回都是 object


###



  