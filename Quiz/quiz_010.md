# code
```.py
s = input("Input a number with unit: ")
n = [int(s) for s in s.split() if s.isdigit()]
powers = []
final = []
Units = ["Tera", "Giga", "Mega", "Kilo", "Unit", "Milli", "Micro", "Nano", "Pico"]
length_lmsg = 20


def power(n):
    count = 0
    for i in range(-12, 0, 3):
        temp = abs(i // 3)
        number = f"0.{(('000 ') * temp)}{str(n[0])} ".ljust(length_lmsg)
        powers.append(f"{number}{Units[count]}{s[1:]}")
        count += 1
    for i in range(0, 15, 3):
        temp = i//3
        number = f"{str(n[0])} {('000 '*temp)} ".ljust(length_lmsg)
        powers.append(f"{number}{Units[count]}{s[1:]}")
        count += 1

    return powers

print("\n".join(power(n)))
```
# Flow diagram
![10](https://user-images.githubusercontent.com/100017195/197777511-a5539c7f-62e3-41f0-86ef-f2e6915bedec.jpeg)

# Test
![Quiz010_Evidence](https://user-images.githubusercontent.com/100017195/197688481-cc0dd639-48b5-4113-9b64-c8b62b585e1b.jpg)
