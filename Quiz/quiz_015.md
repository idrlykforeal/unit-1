# Code

```.py
def open_doors(number:int)->list:
    doors=[]

    for i in range(number):
        doors.append(True)

    for student_num in range(2,number+1):
        for door_index in range(number):
            if (door_index+1)%student_num==0:
                doors[door_index]= not doors[door_index]

    return doors

n=5
count=0
print(f"here are the situation of the doors when there are {n} doors and students: ")
for i in open_doors(n):
    if i==True:
        print("open", end=" ")
        count+=1
    else:
        print("closed", end=" ")
print(f"\nthere are {count} doors open in total when there are {n} doors and students")
```
# Flow diagram
![Comp Science](https://user-images.githubusercontent.com/100017195/197784800-7b8c07e5-3ed2-4dc9-b810-42477cecad3a.jpeg)

# Test results

<img width="950" alt="quiz15" src="https://user-images.githubusercontent.com/100017195/193987566-046f3554-4c36-4a32-915c-c4c2ce17a988.png">
