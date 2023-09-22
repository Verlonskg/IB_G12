# quiz_070

## Paper Program
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_071.jpg)


## Code Evidence
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_071_test.jpg)

## Code

```.py
from random import randint

def ipv6m(N:int):
    output = []
    for i in range(N):
        ipv6=""
        for x in range(8):
            a = ""
            hex = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "B", "C", "D", "E", "F"]
            for y in range(4):
                b = randint(0, 14)
                a += hex[b]
                if len(a)==4 and a != 7:
                    a += ":"
                    ipv6 += a
                if len(a) == 4 and a == 7:
                    ipv6 += a
        output.append(ipv6)
    return(output)
```
