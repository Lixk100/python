# 实验步骤  
- 命令行模式 `$vim average.py`   
- 按i进入插入模式  
```python
#!/usr/bin/env python3                          //指定编辑器
N = 10
sum = 0
count = 0
print("please input 10 numbers:")
while count < N:                               //while语法
    number = float(input())
    sum = sum + number
    count = count + 1
average = sum / N
print("N = {}, Sum = {}".format(N, sum))       //字符串格式化
print("Average = {:.2f}".format(average))  
```
[while语法与字符串格式化](https://github.com/liytgy/python/blob/master/START/while%E4%B8%8E%E5%AD%97%E7%AC%A6%E4%B8%B2%E6%A0%BC%E5%BC%8F%E5%8C%96.md)  👈👈👈知识点  
- 按esc进入普通模式  
- 进入命令行模式：wq保存退出  
- 加执行权限  
`$sudo chmod +x average.py`   ~~(也可以不加sudo)~~  
- 执行文件  `$./average.py`  
```python
1.2
3.4
3.5
33.2
2
4
6
2.4
4
5.5
N = 10, Sum = 65.2
Average = 6.52
```
