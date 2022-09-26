# Code
```.py
# print the calendar from a given month in 2022.

def bestMonth(month:int):
    day=["Mon", "Tues", "Wed", "Thurs", "Fri", "Sat", "Sun"]
    start=[5, 1, 1, 4, 6, 2, 4, 0, 3, 5, 1, 3]
    days = []
    a=1
    x=start[month-1]
    if month in [1, 3, 5, 7, 8, 10, 12]:
        repeat=31
    if month == 2:
        repeat=28
    if month in [4, 6, 9, 11]:
        repeat=30
    for i in range(repeat):
        days.append([a, day[x]])
        a += 1
        x += 1
        if x == 6:
            x = 0
    return days

month=int(input("Please enter the number of the month that you would like to get the calendar of: "))

count=0
for i in bestMonth(month):
    print(i, end=" ")
    count+=1
    if count%5==0:
        print()
```

# Test

<img width="935" alt="quiz11" src="https://user-images.githubusercontent.com/100017195/192197522-d5f4fe75-88c9-49af-a7f9-25f2659e2f64.png">
