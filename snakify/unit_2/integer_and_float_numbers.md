# Last digit of integer

## Code
```.py
a = int(input())
print(a%10)
```

## Tests

![](2_1_1.png)
![](2_1_2.png)
![](2_1_3.png)

# Two digits

## Code
```.py
a = int(input())
first= int((a-(a%10))/10)
print(first,a%10)
```

## Tests

![](2_2_1.png)
![](2_2_2.png)
![](2_2_3.png)

# Swap digits

## Code
```.py
a = int(input())
tenth= int((a-(a%10))/10)
one=a%10
print(str(one)+str(tenth))
```

## Tests

![](2_3_1.png)
![](2_3_2.png)

# Last two digits

## Code
```.py
a = int(input())
print(a%100)
```

## Tests

![](2_4_1.png)
![](2_4_2.png)

# Tens digit

## Code
```.py
a = int(input())
tenth= int(a//10 % 10)
print(tenth)
```

## Tests

![](2_5_1.png)
![](2_5_2.png)
![](2_5_3.png)

# Sum of digits

## Code
```.py
a = int(input())
hundreds= int(a//100)
tenth= int(a//10 % 10)
one=a%10

print(hundreds+tenth+one)
```

## Tests

![](2_6.png)

# Reverse three digits

## Code
```.py
a = int(input())
hundreds= int(a//100)
tenth= int(a//10 % 10)
one=a%10

print(str(one)+str(tenth)+str(hundreds))
```

## Tests

![](2_7_1.png)
![](2_7_2.png)

# Merge two numbers

## Code
```.py
a= int(input())
b= int(input())

a1= str(a//10)
a2= str(a%10)
b1= str(b//10)
b2= str(b%10)

print (a1+b1+a2+b2)
```

## Tests

![](2_8_1.png)
![](2_8_2.png)

# Cyclic rotation

## Code
```.py
a = int(input())
a1=a//100
a2=a%100

print(str(a2)+str(a1))
```

## Tests

![](2_9_1.png)
![](2_9_2.png)

# Fractional part

## Code
```.py
a = float(input())
dec=a%1
print(dec)
```

## Tests

![](2_10.png)

# First digit after decimal point

## Code
```.py
a = float(input())
dec1=(a%1*10)//1

print(dec1)
```

## Tests

![](2_11_1.png)
![](2_11_2.png)
![](2_11_3.png)

# Car route

## Code
```.py
from math import ceil
n = int(input())
m = int(input())
days=ceil(m/n)

print(days)
```

## Tests

![](2_12_1.png)
![](2_12_2.png)

#  Day of week

## Code
```.py
a = int(input())
day=(a-4)%7
print(day)
```

## Tests

![](2_13_1.png)
![](2_13_2.png)
![](2_13_3.png)

# Digital clock

## Code
```.py
time = int(input())
hours= time//60
minutes= time%60

print(hours, minutes)
```

## Tests

![](2_14.png)

# Total cost
a = int(input())
b = int(input())
n = int(input())

dollars = n*a + (n*b)//100
cents = (b*n) % 100

print(dollars, cents)
## Code
```.py

```

## Tests

![](2_15_1.png)
![](2_15_2.png)

# Century

## Code
```.py
from math import ceil

year = int(input())
cent = ceil(year/100)

print(cent)
```

## Tests

![](2_16_1.png)
![](2_16_2.png)
![](2_16_3.png)

# Snail

## Code
```.py
from math import ceil

H = int(input())
a = int(input())
b = int(input())

days= ceil((H-a)/(a-b)+1)

print(days)
```

## Tests

![](2_17_1.png)
![](2_17_2.png)
![](2_17_3.png)

# Clock face - 1

## Code
```.py
h = int(input())
m = int(input())
s = int(input())

degrees= (h + m/60 + s/3600)*30

print(degrees)
```

## Tests

![](2_18_1.png)
![](2_18_2.png)

# Clock face - 2

## Code
```.py
h=float(input())

print((h*12)%360)
```

## Tests

![](2_19_1.png)
![](2_19_2.png)
![](2_19_3.png)
![](2_19_4.png)
