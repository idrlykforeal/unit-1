Generate random password for users
# Code
```.py
import random

num_digits= int(input("Please input the digits you want your password to be: "))
if_symbols=input('Please type True if you would like to have digits in your password: ')

for i in range(10):
    password = []
    if if_symbols.title()=="True":
        for x in range(num_digits):
            digit = random.randint(48, 122)
            while 57 < digit < 65 or 90 < digit < 97:
                digit = random.randint(48, 122)
            rand_chr = chr(digit)
            password.append(rand_chr)
    else:
        for x in range(num_digits):
            digit = random.randint(65, 122)
            while 90 < digit < 97:
                digit = chr(random.randint(65, 122))
            rand_chr=chr(digit)
            password.append(rand_chr)
    for element in password:
        print(element, end="")
    print()

```

# Flow chart

![IMG_0400](https://user-images.githubusercontent.com/100017195/191042882-bd912c71-0106-4198-9701-89e181bac97e.jpeg)

# Tests

<img width="947" alt="quiz7" src="https://user-images.githubusercontent.com/100017195/192192508-2ac1f273-da0e-4c0b-b654-ce92d4f95f3c.png">

