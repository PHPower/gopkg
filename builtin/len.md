## func len(v Type) int

参数列表：

- v Type 要计算的值

返回值：

- int 返回 v 的长度

功能说明：

len 内建函数返回 v 的长度，这取决于具体类型：

~~~
数组：v 中元素的数量。
数组指针：*v 中元素的数量（即使 v 为 nil）。
切片或映射：v 中元素的数量；若 v 为 nil，len(v) 即为零。
字符串：v 中字节的数量。
信道：信道缓存中队列（未读取）元素的数量；若 v 为 nil，len(v) 即为零。
~~~