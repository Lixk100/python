# 正打印  

```python3  
#!/usr/bin/env python3
n = int(input("Enter the number of rows: "))
i = 1
while i <= n:
    print("*" * i)
    i += 1
```
效果：  
```
*
**
***
****
*………共N个……*    //n取决于你输入的行数     
```
 

# 倒置星星     
```python3    
#!/usr/bin/env python3
row = int(input("Enter the number of rows: "))
n = row
while n >= 0:
    x =  "*" * n
    print(x)
    n -= 1
```  

对应效果  
```
*………共N个………………*  
*………N-1个……………*  
……以此类推………  
***
**
*
``` 
# 三角星星图案三
```
#!/usr/bin/env python3
row = int(input("Enter the number of rows: "))
n = row
while n >= 0:
    x = "*" * n
    y = " " * (row - n)
    print(y + x)
    n -= 1
```
效果  
![](https://github.com/liytgy/python/blob/master/START/photo/%E6%98%9F%E6%98%9F%E5%9B%BE%E6%A1%883.png)
