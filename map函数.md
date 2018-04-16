#map函数
#####map() 会根据提供的函数对指定序列做映射。
#####第一个参数 function 以参数序列中的每一个元素调用 function 函数，返回包含每次 function 函数返回值的新列表。

	li = [1,3,5,7,9]
	ls = [2,4,6,8,10]
	
	def add(x,y):
    	return x + y
	
	def jiayi(x):
		return x + 1
	
	def chengyier(x):
		res = x*2
		return res
	
	def jiayichengyier(x):
		x = x + 1
		return x ** 2

	def jiayichengyier(x):
        x = jiayi(x)
        return x ** 2
	
	resjiayi = map(jiayi,li)
	print(list(resjiayi))
	
	reschengyiere = map(chengyier,li)
	print(list(reschengyiere))
	
	resjiayichengyier = map(jiayichengyier,li)
	print(list(resjiayichengyier))

	res = map(add,li,ls)
	reslist = list(res)
	print(reslist)

	res = map(jiayichengyier,li)
	print(list(res))