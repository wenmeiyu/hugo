---
title: "Some Code About Manage .xls files."
date: 2018-07-05
draft: false
---

---
- #!/usr/bin/python
- # -*- coding: UTF-8 -*-
 
- import os  
- from pyExcelerator import *  
 
- sourse_path = os.getcwd()  # 当前工作目录
- path =sourse_path+"\data"  # 数据文件夹目录 
- print path
 
- files= os.listdir(path) # 得到数据文件夹下的所有文件名称 
 
- txtName=files[0] # 获取第一个文件名称
- exName=txtName.replace('txt','xls') # 将命名execel文件
- print exName
 
- w = Workbook()  # 创建workbook      
- ws = w.add_sheet('Sheet1')  # 增加一个sheet页'Sheet1'
 
- j=0
- for file in files: #遍历文件夹  
-    fo = open(path+"/"+file)
-    line = fo.readline()
-    line = fo.readline()
-    #循环遍历取值
-    ws.write(0,j,file)    #第一行输入文件名
-    for i in range(1,122):
-       line = fo.readline()
-       m=float(line[7:12])
-       ws.write(i,j,m)
-       i=i+1
-    j=j+1
    
- w.save(exName)
---