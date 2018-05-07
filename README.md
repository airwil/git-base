# git本地项目连接github教程

一、设置Git的user name和email：
$ git config --global user.name "xxx"
$ git config --global user.email xxx@xxx.com

二、生成SSH密钥过程：
1.查看是否已经有了ssh密钥：cd ~/.ssh
如果没有密钥则不会有此文件夹，有则备份删除
2.生存密钥：
$ ssh-keygen -t rsa -C “xxx@xxx.com”

三、在github个人中心setting上添加ssh密钥，这要添加的是“id_rsa.pub”里面的公钥。
 
四、github创建repository

五、本地项目git init

六、git add remote 远程别名 远程项目地址   
例如：git add remote github git@github.com:airwil/easybuild.git

七、git pull 远程别名 分支名    例如：git pull github master

八、git push --set-upstream 远程别名 远程分支  例如：git push --set-upstream github master
