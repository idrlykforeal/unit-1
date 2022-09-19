# Allocating rooms

## Code

```.py
index=int(input("please input your room index from 1-100: "))
if index<0 or index>100:
    index = int(input("please put a valid room index from 1-100: "))
for floor in range(1,11,1):
    for room in range(1,11,1):
        if index==(floor-1)*10+room:
            print(f'Floor{floor} Room{room}')
```
## Flow Diagram

![IMG_8020](https://user-images.githubusercontent.com/100017195/191028726-741ca27b-6f3c-48a5-a5c4-a23bfc878570.jpeg)


## Tests:

![](Screen Shot 2022-09-19 at 3.53.11 PM.png)
