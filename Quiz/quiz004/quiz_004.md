# Determine if the interger equals to the sum of all its digits.

## Code

```.py
num= input('Please input a integer: ')
max_number_tries=5
while num.isdigit()==False and max_number_tries>0:
    num= input('error! please input a 2 digit integer')
    max_number_tries= max_number_tries+1

if max_number_tries!=0:
    print('well done entering an integer')
    sum=0
    for n in num:
        sum=sum+int(n)
    if sum==int(num):
        print("Perfect Number")
    else:
        print("Not Perfect Number")
else:
    print("you ran out of chances to enter an integer")
    exit()
 ```
 
## Flow chart
![IMG_0396](https://user-images.githubusercontent.com/100017195/191035100-88df424a-0ae3-4c64-88ec-0d222d789456.jpeg)
![IMG_0395](https://user-images.githubusercontent.com/100017195/191035113-46ff52c5-6f33-4658-9099-d809ed845ff7.jpeg)

 
## Tests
![](quiz_004.png)
