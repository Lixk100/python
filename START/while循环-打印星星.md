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
