Tax calculator

```.py
#tax calculator
salary=int(input("please input your salary in dollars: "))

if salary>0 and salary<10001:
    taxed=int(salary*0.05)
elif salary>10000 and salary<50001:
    taxed=int(salary*0.1)
elif salary>50000 and salary<100001:
    taxed=int(salary*0.15)
elif salary>100000:
    taxed = int(salary * 0.25)
else:
    print("Please input a positive integer!")


print(f'the tax you need to pay is {taxed} dollars.')

```
