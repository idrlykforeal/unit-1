# Code

```.py
def blackboxThree(given:str)->str:
    output=""
    x=[]

    for letter in given.lower():
        if letter.isalpha():
            found=False
            for element in x:
                if element[0]==letter:
                    element[1]+=1
                    found=True
                    output+= str(element[1])
            if found == False:
                x.append([letter,1])
                output += "1"
        else:
            output+=letter
    return output


print(blackboxThree("hello world"))
```
# Flow diagram
![Comp Science](https://user-images.githubusercontent.com/100017195/197787627-5b5aae73-6515-44a2-b0b9-0d732beebe2a.jpeg)


# Test
<img width="978" alt="16" src="https://user-images.githubusercontent.com/100017195/197770621-dcdc4387-fa16-47b3-a35f-4c57059cca50.png">
