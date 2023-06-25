# python-task-2
Assignment
 
 
 1. import re
password = "D@t@Science2023"
flag = 0
while True:
	if (len(password)<=10):
		flag = -1
		break
	elif not re.search("[a-z]", password):
		flag = -1
		break
	elif not re.search("[A-Z]", password):
		flag = -1
		break
	elif not re.search("[0-10]", password):
		flag = -1
		break
	elif not re.search("[_@$]" , password):
		flag = -1
		break
	elif re.search("\s" , password):
		flag = -1
		break
	else:
		flag = 0
		print("Valid Password")
		break

if flag == -1:
	print("Not a Valid Password ")


2.seq = ['marvel','dog','salad','cat','great']

sseq = " ".join(seq)

filtered = lambda x: True if sseq.startswith('m') else False

filtered_list = filter(filtered, seq)

print('Words are:')
for a in filtered_list:
    print(a)


 3.   numstr = '100' 
>>> numstr.isnumeric()
True
>>> numstr = '\u0034'
>>> numstr.isnumeric()
True
>>> numstr = '\u00BD' 
>>> numstr.isnumeric()
True
>>> numstr = '3/4' 
>>> numstr.isnumeric()
True


4.def Sort_Tuple(tup):

	
	lst = len(tup)
	for i in range(0, lst):

		for j in range(0, lst-i-1):
			if (tup[j][1] > tup[j + 1][1]):
				temp = tup[j]
				tup[j] = tup[j + 1]
				tup[j + 1] = temp
	return tup

tup = [("mango",99),("orange",80), ("grapes", 1000)]

print(Sort_Tuple(tup))


5. data=[1,2,3,4,5,6,7,8,9,10]

result = [i*i for i in data if i%2!=0]

print(result)


6. import math
 
def cubic_root(n):
    return round(math,(math.log(n)1def cubic_root(n):
    
    x = n
    y = (2 * x + n / x**2) / 3
 

    while abs(x - y) >= 0.000001:
        x = y
        y = (2 * x + n / x**2) / 3
 
    return y
 
 
n = 3
print("Cubic root of", n, "is", round(cubic_root(n), 6))/3), 6);
 
n = 3
print("Cubic Root of", n, "is", cubic_root(n))
 
n = 8
print("Cubic Root of", n, "is", cubic_root(n))




7.num = int (input (Enter any number to test whether it is odd or even:)

if (num % 2) == 0:

           print (“The number is even”)

else:

              print (“The provided number is odd”)



8. list1 = [1,2,3,4,5,6,7,8,9,10]
for num in list1:
if num % 2 != 0:
	print'num'


9.test_list = [1,2,3,4,5,6,-1,-2,-3,-4,-5,0]

print("The original list is : " + str(test_list))


res = sorted(test_list, key = lambda i: 0 if i == 0 else -1 / i)


print("Result after performing sort operation : " + str(res))

