##git操作流程

####使用`git init`命令创建一个.git文件夹

####使用`git config --global user.name "name"`以及`git config --global user.email "email"`来设置自己的名字和邮箱

####使用`git config --list`查看配置文件

####使用`git status`查看状态

####使用`git add [当前路径]`将文件保存到暂存区

####使用`git commit -m "一些注释"`来提交暂存区代码

####使用`.`代表所有文件；`git add .`代表将所有文件都提交到暂存区

####使用`git log`来查看保存日志
	使用`git log --oneline`在一行显示

####合并以上操作：
	git commit -a -m "添加注释"
	注意：新建的文件不能使用连写；只有修改的文件可以使用连写

####暂存区，同一个文件只会保存最新版本，不同的文件可以共存