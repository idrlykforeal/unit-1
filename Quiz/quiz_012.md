# Code
```.py
def mulTable(num:int):
    out=[]
    for i in range(1,10):
        mult=num*i
        out.append(f"{num} x {i} = {mult}")
    return out

user_input=int(input("please input your number that you would see the multiplication table of: "))
for i in mulTable(user_input):
    print(i)
```
# Flow diagram
![Comp Science](https://user-images.githubusercontent.com/100017195/197781698-85a70f35-543c-463d-a09a-a3d9edb0b37b.jpeg)

# Test
<img width="958" alt="quiz12" src="https://user-images.githubusercontent.com/100017195/192907544-2e29b3bc-6dc8-44c6-b7bb-22e8b0a9513e.png">
