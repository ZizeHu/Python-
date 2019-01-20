# Python-
个人于2019.1月开始的踩坑之路
#列表
list=[]
#元组
Tuple=()
#集合
set={}
#字典
Dictionary={}
dict={
    'Name':'梓泽',
    'Age':19,
    'Sex':'男'
}
print(dict['Name'])
#lambda函数
try:
    sum=lambda  num1,num2:num1+num2
    print('相加值：%s'% sum(-10,19))
except:
    print("输入有误无法计算")

bonus1 = 100000 * 0.1
bonus2 = bonus1 + 100000 * 0.500075
bonus4 = bonus2 + 200000 * 0.5
bonus6 = bonus4 + 200000 * 0.3
bonus10 = bonus6 + 400000 * 0.15

i = int(input('input gain:\n'))
if i <= 100000:
    bonus = i * 0.1
elif i <= 200000:
    bonus = bonus1 + (i - 100000) * 0.075
elif i <= 400000:
    bonus = bonus2 + (i - 200000) * 0.05
elif i <= 600000:
    bonus = bonus4 + (i - 400000) * 0.03
elif i <= 1000000:
    bonus = bonus6 + (i - 600000) * 0.015
else:
    bonus = bonus10 + (i - 1000000) * 0.01
print ('bonus = ',bonus)
