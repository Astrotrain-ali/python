#filter函数
#####filter() 函数用于过滤序列，过滤掉不符合条件的元素，返回由符合条件元素组成的新列表。
#####该接收两个参数，第一个为函数，第二个为序列，序列的每个元素作为参数传递给函数进行判，然后返回 True 或 False，最后将返回 True 的元素放到新列表中。

####计算列表中的奇数
	li = [1,2,3,4,5,6,7,8,9,10]
	def test(x):
	    return x %2 == 1
	
	res = filter(test,li)
	print(list(res))

####取出中包含sb的元素
	li = ["sb_baoma","sb_benchi","sb_aodi","fute"]	
	def test1(x):
    return "sb" in x

	res = filter(test1,li)
	print(list(res))
####取出不包含sb的元素
	li = ["sb_baoma","sb_benchi","sb_aodi","fute"]	
	def test1(x):
    return "sb" not in x

	res = filter(test1,li)
	print(list(res))

####取出不以sb开头的元素
	li = [1,2,3,4,5,6,7,8,9,10]
	res = filter(lambda x:not x.startswith("sb"),li)
	print(list(res))

####取出age大于18的元素
    people = [
        {'name':'ali','age':18},
        {'name':'ayisha','age':20},
    ]
    
    
    print(list((filter(lambda p:p['age'] <= 18,people))))