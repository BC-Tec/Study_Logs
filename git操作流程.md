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



注意：

git add -A和 git add . git add -u在功能上看似很相近，但还是存在一点差别

git add . ：他会监控工作区的状态树，使用它会把工作时的所有变化提交到暂存区，包括文件内容修改(modified)以及新文件(new)，但不包括被删除的文件。

git add -u ：他仅监控已经被add的文件（即tracked file），他会将被修改的文件提交到暂存区。add -u 不会提交新文件（untracked file）。（git add --update的缩写）

git add -A ：是上面两个功能的合集（git add --all的缩写）