# Cypher with letter shift

## Code
```.py
string=input("please input your string: ").lower()
shift=int(input("please input the shift you would like to make: "))
shift = shift%26

for letter in string:
    ord_1=ord(letter)
    if ord_1==32:
        ord_2=32
    else:
        ord_2=ord_1+shift
        if ord_2>122:
            ord_2-=26
    print(chr(ord_2), end="")
```

## Flow Diagram
![quiz_009_flow](https://user-images.githubusercontent.com/100017195/191261140-44a1c40b-b436-4c76-9d72-72bf90af3778.jpeg)

## Test
<img width="820" alt="quiz_009" src="https://user-images.githubusercontent.com/100017195/191260831-b2d9e9ec-7e3e-4058-ada4-b93824664fd4.png">
