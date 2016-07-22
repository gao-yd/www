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

####对比文件的变化`git diff`

####git reset --[c]  c为参数

	hard head:回到上一次提交的代码
	hard head^^:回到倒数第二次提交的代码
	hard head~1:回到最近一次提交的前一次
	hard [版本号]：会退到具体的版本号


####新建一个名称为`.gitignore`文件里面写入`/.gitignore`;`.gitignore`用来告诉git哪些文件不需要被提交

####`git reflog`记录了用户的所有提交和回退;
	通过reset+版本号可以回到回退之前的版本。

####`git clone [仓储地址]`克隆整个版本仓库中的代码
如果不需要下载整个仓储，只是需要下载最新的版本，可以加上参数--depath 1;

- - - 

####git分支

	-git默认分支为master；
	-使用`git branch`可以查看默认分支
	-使用`git branch dev`新建一个名字为dev分支
	-git checkout dev 切换到dev分支
	-使用`git merge dev`把当前分支与dev分支进行合并
	-git branch -d dev删除dev分支，此操作不能再dev分支下使用
	-git checkout -b dev 创建dev分支，并切换到dev分支下

- - - 
####github 和 git

	git push [地址] master  将本地仓储添加到服务器的master分支中

	-github有个特殊的分支gh-pages
	-代码提交到这个分支中可以直接在线浏览
####创建变量

	git remote origin[地址]
	变量中储存的是地址