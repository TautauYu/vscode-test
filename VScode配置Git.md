# VSCODE配置Git
## 安装Git
## Git配置
打开Git的bash配置全局设置
用户名
* git config --global user.name "用户名"
邮箱
* git config --global user.email "xxx@email.com"
记得提交的邮箱即密码
* git config --global credential.helper store

## Vscode配置
1.使用vscode打开要上传的文件夹，文件夹内可以有文件也可没有；
2.若没有文件，则新建文件并将之存储在上述文件内；
3.点击vscode右侧的git图标，初始化存储库；
4.回到文件夹界面，点击鼠标右键并选择Git Bash here，输入如下命令：
GitHub项目地址(GitHub中已经创建repository)
* git remote add origin https://github.com/TautauYu/XXX.git
初始化仓库
* git pull --rebase origin master
提交代码到仓库
* git push -u origin master
** 若出现“https”问题，则将