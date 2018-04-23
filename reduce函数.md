#reduce函数
#####reduce() 函数会对参数序列中元素进行累积。

#####函数将一个数据集合（链表，元组等）中的所有数据进行下列操作：用传给reduce中的函数 function（有两个参数）先对集合中的第 1、2 个元素进行操作，得到的结果再与第三个数据用 function 函数运算，最后得到一个结果。
#####python2.6版本可以直接用。3.x版本则需要导入模块
from functools import reduce

	from functools import reduce
	
	num_li = [1,2,3,100]
	print(reduce(lambda x,y:x*y,num_li))
	print(reduce(lambda x,y:x+y,num_li))