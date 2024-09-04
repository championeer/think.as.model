# Jackfrued/Python-100-Days

![rw-book-cover](https://readwise-assets.s3.amazonaws.com/static/images/article0.00998d930354.png)

## Metadata
- Author: [[github.com]]
- Full Title: Jackfrued/Python-100-Days
- Category: #articles
- URL: https://github.com/jackfrued/Python-100-Days/blob/master/Day01-15/04.%E5%BE%AA%E7%8E%AF%E7%BB%93%E6%9E%84.md

## Highlights
- 循环结构就是程序中控制某条或某些指令重复执行的结构。在Python中构造循环结构有两种做法，一种是for-in循环，一种是while循环。
- 如果明确的知道循环执行的次数或者要对一个容器进行迭代（后面会讲到），那么我们推荐使用for-in循环
- range(101)：可以用来产生0到100范围的整数，需要注意的是取不到101。
  range(1, 101)：可以用来产生1到100范围的整数，相当于前面是闭区间后面是开区间。
  range(1, 101, 2)：可以用来产生1到100的奇数，其中2是步长，即每次数值递增的值。
  range(100, 0, -2)：可以用来产生100到1的偶数，其中-2是步长，即每次数字递减的值。
- 如果要构造不知道具体循环次数的循环结构，我们推荐使用while循环。while循环通过一个能够产生或转换出bool值的表达式来控制循环，表达式的值为True则继续循环；表达式的值为False则结束循环。
- 使用了break关键字来提前终止循环，需要注意的是break只能终止它所在的那个循环，这一点在使用嵌套的循环结构（下面会讲到）需要引起注意。除了break之外，还有另一个关键字是continue，它可以用来放弃本次循环后续的代码直接让循环进入下一轮。
# Jackfrued/Python-100-Days

![rw-book-cover](https://readwise-assets.s3.amazonaws.com/static/images/article0.00998d930354.png)

## Metadata
- Author: [[github.com]]
- Full Title: Jackfrued/Python-100-Days
- Category: #articles
- URL: https://github.com/jackfrued/Python-100-Days/blob/master/Day01-15/04.%E5%BE%AA%E7%8E%AF%E7%BB%93%E6%9E%84.md

## Highlights
- 循环结构就是程序中控制某条或某些指令重复执行的结构。在Python中构造循环结构有两种做法，一种是for-in循环，一种是while循环。
- 如果明确的知道循环执行的次数或者要对一个容器进行迭代（后面会讲到），那么我们推荐使用for-in循环
- range(101)：可以用来产生0到100范围的整数，需要注意的是取不到101。
  range(1, 101)：可以用来产生1到100范围的整数，相当于前面是闭区间后面是开区间。
  range(1, 101, 2)：可以用来产生1到100的奇数，其中2是步长，即每次数值递增的值。
  range(100, 0, -2)：可以用来产生100到1的偶数，其中-2是步长，即每次数字递减的值。
- 如果要构造不知道具体循环次数的循环结构，我们推荐使用while循环。while循环通过一个能够产生或转换出bool值的表达式来控制循环，表达式的值为True则继续循环；表达式的值为False则结束循环。
- 使用了break关键字来提前终止循环，需要注意的是break只能终止它所在的那个循环，这一点在使用嵌套的循环结构（下面会讲到）需要引起注意。除了break之外，还有另一个关键字是continue，它可以用来放弃本次循环后续的代码直接让循环进入下一轮。
