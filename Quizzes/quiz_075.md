# quiz_075

## Paper Program
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_075.jpg)


## Code Evidence
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_075_test.jpg)

## Code

```.py
def binary(num):
    output = ""
    for i in range(8):
        output += str((num//2**i)%2)
    return output[::-1]

def osi_model(data):
    output = ""
    for i in range(len(data)):
        output += binary(ord(data[i]))
        output += " "
    return output
```
