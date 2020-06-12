1. vim cs.py
``` 
#!/usr/bin/env python3
a, b = 0, 1
while b < 100:
    print(b)
   a, b = b, a + b  
```
运算方式：
 输出b，
 计算先计算b = a+b ，后计算a = b    
 
# 可以这样理解，Python 中赋值语句执行时会先对赋值运算符右边的表达式求值，然后将这个值赋值给左边的变量。
 
2. print()  
python3中print()可以调用换行符  
