# Python-15-
Python学习笔记(15)
# p50 获取1列表中的指定元素
lst=['hello','world',98,'hello','world',234]
#获取索引为2的元素
print(lst[2]) #输出为98
#获取索引为-3的元素
print(lst[-3]) #输出为hello
#获取索引为10的元素
print(lst[10]) #out of range



# p51 获取列表中的多个元素的切片
#语法格式
#列表名[start:stop:step]
lst=[10,20,30,40,50,60,70,80,]
print(lst[1:6:1])
#输出为[20,30,40,50,60]
print('原列表'，id(lst))
lst2=lst[1:6:1]
print('切片片段：'id(lst2))# 将原列表当中的一段切片给拷贝
print(lst[1:6]) #默认步长为1
print(lst[1:6:]) #    也是1
print(lst[1:6:2]) #输出20，40，60
print(lst[:6:2]) #输出10，30，50
print(lst[1::2]) #输出为20，40，60，80

#当step为负数
print(lst[::-1]) #输出为80，70，60，50，40，30，20，10
print(lst[7::-1]) #输出同上
print(lst[6:0:-2]) #70,50,30



# p52 列表元素的判断及遍历
print('p' in 'python') #True
print('k' not in 'python') #True

lst=[10,20,'python','hello']
print(10 in lst) #True
print(100 in lst) #False
print(10 not in lst) #False
print( 100 not in lst) #True

#至于遍历就使用for迭代变量(目前学到的是字符串和列表)in列表名：
for item in lst:
    print(item)
