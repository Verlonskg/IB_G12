# quiz_077

## Paper Program
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_077.jpg)


## Code Evidence
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_077_test.jpg)

## Code

```.py
def parity_check(data: str):
    output = []
    for i in range(1, len(data)):
        if data[i] == "1":
            output.append(1)

    if len(output)%2 < 1:
        return "True"
    else:
        return "False"
```
