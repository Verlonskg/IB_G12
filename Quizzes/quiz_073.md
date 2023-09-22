# quiz_073

## Paper Program
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_073.jpg)

## Code Evidence
![](https://github.com/Verlonskg/IB_G12/blob/main/Files/quizzes/quiz_073_test.jpg)

## Code

```.py
from random import randint

class RoutingTable:
    def __init__(self, mac:str):
        self.routing_table = {}
        self.mac_in = mac

    def check_mac(self):
        return len(self.mac_in) == 17 and self.mac_in.count(":") == 5

    def ipv6m(self):
        ipv6 = ""
        for x in range(8):
            a = ""
            hex = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "B", "C", "D", "E", "F"]
            for b in range(4):
                b = randint(0, 14)
                a += hex[b]
                if len(a) == 4 and x != 7:
                    a += ":"
                    ipv6 += a
                if len(a) == 4 and x == 7:
                    ipv6 += a
        return ipv6

    def get_ip(self):
        if self.check_mac():
            if self.mac_in in self.routing_table.keys():
                ip_out = self.routing_table[self.mac_in]
            else:
                while True:
                    ip = self.ipv6m()
                    if not ip in self.routing_table.values():
                        self.routing_table[self.mac_in] = ip
                        ip_out = ip
                        break
                    print(self.routing_table)
            return self.routing_table
```
