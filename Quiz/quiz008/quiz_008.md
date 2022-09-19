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
<img width="820" alt="quiz_008" src="https://user-images.githubusercontent.com/100017195/191028896-8c4b9ee8-952c-4483-97bc-5727b3029cec.png">
