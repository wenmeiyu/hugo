---
title: "Some Environment Notes"
date: 2018-07-05
draft: false
---

---
- 搭建gogs环境：
 
- "# ielts" 
- https://gogs.io/
- http://210.75.252.89:3000/

- 从命令行创建一个新的仓库
- touch README.md
- git init
- git add README.md
- git commit -m "first commit"
- git remote add origin http://210.75.252.89:3000/wenmy/Documents.git
- git push -u origin master
- 
- 从命令行推送已经创建的仓库
- git remote add origin http://210.75.252.89:3000/wenmy/Documents.git
- git push -u origin master

---
- 搭建背单词环境：
 
- wmic environment create UserName="<system>",name="GIT",VariableValue="C:\git"
- wmic environment where 'UserName="<system>" and name = "Path"' set VariableValue="%PATH%;%GIT%\mingw64\bin;%GIT%\usr\bin;"
- mkdir %USERPROFILE%\.ssh
- sysdm.cpl
- git clone https://github.com/ikey4u/quick-vim-setup.git %USERPROFILE%\vimfiles
- git clone git@github.com:wenmeiyu/hugoblog.git
- git clone hugo:wenmeiyu/ielts.git
 
- echo "# ielts" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git remote add origin hugo:wenmeiyu/ielts.git
- git push -u origin master

- git remote add origin hugo:wenmeiyu/ielts.git
- git push -u origin master
 
- git config --global user.email "1157515766@qq.com"
- git config --global user.name "wenmeiyu"
 
- 日常命令：
- git add filename.md
- git commit -m "first commit info"
- git push -u origin master

- 单词地址
- https://github.com/lw19960617/IELTS
- https://github.com/wenmeiyu/ielts
- 

---
- 搭建hogo blog环境：
- hugo:wenmeiyu/hugo.git
- hugo:wenmeiyu/wenmeiyu.github.io.git
- hugo new site hugoblog
- cd hugoblog

- git init
- git config --local user.name wenmeiyu
- git config --local user.email 1157515766@qq.com
- git config --global core.quotepath false
- git remote add origin hugo:wenmeiyu/hugo.git
- git submodule add hugo:wenmeiyu/wenmeiyu.github.io.git public
- git add .
- git commit -m "blog init setup"
- git push origin master

- cd public
- git config --local user.name wenmeiyu
- git config --local user.email 1157515766@qq.com

- curl https://raw.githubusercontent.com/ikey4u/hugo-guide/master/deploy.sh -o deploy.sh

- git clone https://github.com/shenoybr/hugo-goa
- git clone  https://github.com/humboldtux/startbootstrap-clean-blog

- 日常命令：
- hugo new fileclass/filename.md
- bash deploy.sh

- 博客地址
- https://wenmeiyu.github.io/
- just4tuts.github.io
- lw19960617.github.io








