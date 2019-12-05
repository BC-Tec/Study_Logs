# [总结篇——git本地仓库上传更新到github]

一、将需要上传的文件放到一个新建的文件夹下

二、右击找到Git Bash Here，弹出git命令框

三、初始化git

　　$git init

四、将文件添加到本地仓库

　　$git add --all

五、提交到本地仓库

　　$git commit -m "首次提交"

六、与GitHub上的分支建立链接

　　$git remote add origin https://github.com/*****/shop.git

七、将刚刚提交的文件推送到GitHub上

　　$git pull --rebase origin master

　　$git push -u origin master -f