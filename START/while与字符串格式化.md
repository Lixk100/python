# while 是使用一个表达式作为判断的条件，如果条件不能够达成则停止循环：

`w = 20
while w > 1:
    print(w)
    w -= 1`
这个循环中判断条件为 w > 1，当条件不满足的时候就停止循环。当 w 的值小于等于 1 的时候，循环退出。这里要注意 w -= 1，等同于 w = w - 1。

下一个程序我们写入 /home/1.py，来计算投资，使用 Vim 输入以下代码：
```
#!/usr/bin/env python3
amount = float(input("Enter amount: "))  # 输入数额
inrate = float(input("Enter Interest rate: "))  # 输入利率
period = int(input("Enter period: "))  # 输入期限
value = 0
year = 1
while year <= period:
    value = amount + (inrate * amount)
    print("Year {} Rs. {:.2f}".format(year, value))
    amount = value
    year = year + 1
```
运行程序：
```
$ chmod +x 1.py  
$ ./1.py  
Enter amount: 10000  
Enter Interest rate: 0.14  
Enter period: 5  
Year 1 Rs. 11400.00  
Year 2 Rs. 12996.00  
Year 3 Rs. 14815.44  
Year 4 Rs. 16889.60  
Year 5 Rs. 19254.15
```
- while year <= period: 的意思是，当 year 的值小于等于 period 的值时，下面的语句将会一直循环执行下去，直到 year 大于 period 时停止循环。

- Year {} Rs. {:.2f}".format(year, value) 称为字符串格式化，大括号和其中的字符会被替换成传入 str.format() 的参数，也即 year 和 value。其中 {:.2f} 的意思是替换为 2 位精度的浮点数。
