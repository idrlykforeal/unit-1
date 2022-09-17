# is positive

## Code
```.py
a = int(input())
if a>0:
    print('YES')
else:
    print('NO')
```

## Tests

![](.png)


# is odd

## Code
```.py
a = int(input())
if a%2!=0:
    print('YES')
else:
    print('NO')
```

## Tests

![](.png)

# is even

## Code
```.py
a = int(input())
if a%2==0:
    print('YES')
else:
    print('NO')
```

## Tests

![](.png)

# ends on seven

## Code
```.py
a = int(input())
if a%10==7:
    print('YES')
else:
    print('NO')
```

## Tests

![](.png)

# minimum of two numbers

## Code
```.py
a = int(input())
b = int(input())

if a>b:
    print(b)
else:
    print(a)
```

## Tests

![](.png)

# are both odd

## Code
```.py
a = int(input())
b = int(input())
if a%2!=0 and b%2!=0:
    print('YES')
else:
    print("NO")
```

## Tests

![](.png)

# at least one odd

## Code
```.py
a = int(input())
b = int(input())
if a%2!=0 or b%2!=0:
    print('YES')
else:
    print("NO")
```

## Tests

![](.png)

# exactly one odd

## Code
```.py
a = int(input())
b = int(input())
if (a+b)%2!=0:
    print('YES')
else:
    print("NO")
```

## Tests

![](.png)

# sign function

## Code
```.py
x = int(input())
if x >0:
    print(1)
elif x<0:
    print(-1)
else:
    print(0)
```

## Tests

![](.png)

# numbers in ascending order

## Code
```.py
a = int(input())
b = int(input())
c = int(input())

if a<b<c:
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)

# is three digit

## Code
```.py
a = int(input())
if 100<=a<=1000:
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)

# minimum of three numbers

## Code
```.py
a = int(input())
b = int(input())
c = int(input())

if a<b:
    if a<c:
        print(a)
    else:
        print(c)
else:
    if b<c:
        print(b)
    else:
        print(c)
```

## Tests

![](.png)

# equal numbers

## Code
```.py
a = int(input())
b = int(input())
c = int(input())
i=0
if a==b or a==c or b==c:
    i=2
if a==b==c:
    i=3
print(i)

```

## Tests

![](.png)

# Rook move

## Code
```.py
a = int(input())
b = int(input())
a1 = int(input())
b1 = int(input())

if a==a1 or b==b1:
    print("YES")
else:
    print('NO')
```

## Tests

![](.png)


# Chess board - black square

## Code
```.py
a = int(input())
b = int(input())

if (a+b)%2==0:
    print('BLACK')
else:
    print("WHITE")
```

## Tests

![](.png)

# Chess board - same color

## Code
```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())
if (a+b)%2==0:
    color1=1
else:
    color1=0
    
if (c+d)%2==0:
    color2=1
else:
    color2=0
    
if color1==color2:
    print('YES')
else:
    print('NO')

```

## Tests

![](.png)

# Distance to closest point

## Code
```.py
a = int(input())
b = int(input())
c = int(input())

if abs(b-a)>abs(c-a):
    print(abs(c-a))
else:
    print(abs(b-a))
```

## Tests

![](.png)

# Digits in ascending order

## Code
```.py
a = int(input())
hundreds=a//100
tens= a%100//10
ones= a%10


if hundreds<tens<ones:
    print('YES')
else:
    print('NO')
```

## Tests

![](.png)

# Four-digit palindrome

## Code
```.py
a = int(input())

if a//1000==a%10 and (a//100)%10==(a%100)//10:
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)

# King move


## Code
```.py
x = int(input())
y = int(input())
x1 = int(input())
y1 = int(input())

if abs(x - x1) <= 1 and abs(y - y1) <= 1:
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)

# Bishop moves

## Code
```.py
x = int(input())
y = int(input())
x1 = int(input())
y1 = int(input())

if abs(x-x1)==abs(y-y1):
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)

# Queen move

## Code
```.py
x = int(input())
y = int(input())
x1 = int(input())
y1 = int(input())

if abs(x-x1)==abs(y-y1) or x==x1 or y==y1:
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)

# Index of outlier

## Code
```.py
a = int(input())
b = int(input())
c = int(input())

if a==b:
    print(3)
if a==c:
    print(2)
if c==b:
    print(1)
```

## Tests

![](.png)

# Knight move

## Code
```.py
x = int(input())
y = int(input())
x1 = int(input())
y1 = int(input())

if abs(x-x1)==2*abs(y-y1) or 2*abs(x-x1)==abs(y-y1):
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)

# Chocolate bar

## Code
```.py
n = int(input())
m = int(input())
k = int(input())

if (k%m==0 or k%n==0) and m*n>k:
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)

# Leap year

## Code
```.py
year = int(input())

if year%4==0 and year%100!=0:
    print("LEAP")
elif year%400==0:
    print("LEAP")
else:
    print("COMMON")
```

## Tests

![](.png)

# Days in month

## Code
```.py
month= int(input())

if month in [1,3,5,7,8,10,12]:
    print(31)
if month==2:
    print(28)
if month in [4,6,9,11]:
    print(30)
```

## Tests

![](.png)

# Next day

## Code
```.py
month = int(input())
day = int(input())

if (month in [1,3,5,7,8,10] and day==31) or (month==2 and day==28) or (month in [4,6,9,11] and day==30):
    month=month+1
    day=1
elif month==12 and day==31:
    month=1
    day=1
else:
    day=day+1
    
print(month, day)
```

## Tests

![](.png)

# Linear equation

## Code
```.py
a = int(input())
b = int(input())

if a==0 and b==0:
    print("many solutions")
elif a==0 and b!=0 or b%a!=0:
    print('no solution')
else:
    print(b/a)
```

## Tests

![](.png)

# Vertices of rectangle

## Code
```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
x3 = int(input())
y3 = int(input())

if x1==x2:
    x=x3
if x1==x3:
    x=x2
if x3==x2:
    x=x1

if y1==y2:
    y=y3
if y1==y3:
    y=y2
if y3==y2:
    y=y1
    
print(x,y)
```

## Tests

![](.png)

# Sort three numbers

## Code
```.py
a = int(input())
b = int(input())
c = int(input())

if a > b:
    a,b = b,a

if a > c:
    a, c = c, a

if b > c:
    b, c = c, b

print(a,b,c)
```

## Tests

![](.png)

# White pawn move

## Code
```.py
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if y1==1:
    print("NO")
elif x1==x2 and y1==y2:
    print('NO')
elif abs(x1-x2)==1 and y2-y1==1:
    print("YES")
elif y1==2 and x1==x2 and 0<=y2-y1<=2:
    print("YES")
elif x1==x2 and y2-y1==1:
    print("YES")
else:
    print("NO")
```

## Tests

![](.png)
