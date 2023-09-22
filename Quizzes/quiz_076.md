# quiz_076

## Paper Program
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_076.jpg)


## Code Evidence
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_076_test.jpg)

## Code

```.py
def error_check(data):
    output = False
    length = len(data)//3
    for i in range(length):
        if not data[i] == data[i + length] == data[i + 2 * length]:
            output = True
    return output
```
