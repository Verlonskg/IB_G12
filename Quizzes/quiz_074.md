# quiz_074

## Paper Program
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_074.jpg)


## Code Evidence
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_074_test.jpg)

## Code

```.py
import math

def build_data_pkg(Mac_rx, IP_rx, Mac_sx, IP_sx, data):
    length = math.ceil(len(data)/3)
    output = []
    for i in range(length):
        temp = data[4*i : 4*(i+1)]
        output.append(f"{Mac_rx}|{IP_rx}|{Mac_sx}|{IP_sx}|{temp}")
    return output
```
