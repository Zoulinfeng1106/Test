上传远程仓库流程：
1.git add .(上传所有bash所在目录下所有文件)：添加项目文件
2.gitmmit -m "命名“：将项目文件提交到本地仓库
3.git remote add 仓库别名（origin） 仓库地址（https/ssh：选用ssh需要先配置密钥）：本地仓库连接远程仓库
4.git push -u origin（仓库别名） master(分支名)：将本地仓库的内存push到远程仓库

第一次push需要机上-u 第二次则不需要
origin是仓库别名
master是仓库分支名，一个仓库可以有多个分支，每个分支可以上传不同项目文件，但一般都用master

使用”git bash“的位置：上传开启”bash“的当前目录下的文件，即是与”.git“在相同目录下的文件
从远程pull时，拉取的是以仓库名为文件名的文件夹，内部包含分支下项目文件

使用ssh登录，需要先配置登录密钥

帮助blog：https://blog.csdn.net/weixin_43233914/article/details/103502718