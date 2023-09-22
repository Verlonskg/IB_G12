# quiz_072

## Paper Program
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_072.jpg)


## Code Evidence
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_072_test.jpg)

## Code

```.py
from random import randint

def MACadress(num: int):
    output = []
    i = 0
    while i < num:
        hex = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'A', 'B', 'C', 'D', 'E', 'F']
        mac = ""
        for a in range(6):
            for b in range(2):
                mac += hex[randint(0, 14)]
            if a < 5:
                mac += ':'
        if mac not in output:
            output.append(mac)
    i += 1
    return(output)
```
