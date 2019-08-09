#### https://blog.csdn.net/c5113620/article/category/7328319/1?  #java核心类学习
#### https://github.com/phoenixtree2poplar/my-git/blob/master/git-workflow-tutorial.md  #git工作流
#### https://njuferret.github.io/2018/08/24/git-usage/  #git乱码
#### git
```bash
git fetch --all   #强制拉取
git reset --hard origin/master  #强制覆盖本地
git checkout -b dev  #从当前分支创建并切换分支到dev
git push --set-upstream origin dev  #当前分支推送远程分支dev
git push origin :dev  #推送空分支到远程即删除远程分支，需当前不在该分支
git rm -r --cached .  #刷新文件缓存
```
#### gitignore
```bash
target/
.idea/
logs/
```
#### free
```bash
PURGE RECYCLEBIN  #清除回收BIN，gaussdb数据库命令
call mvn -f pom.xml dependency:copy-dependencies  #根据pom.xml拉取仓库
```
#### idea
```bash
Alt + Insert  #set/get; 构造方法;  toString; 重写方法。。。
Ctrl+Alt+T  #将代码包在一个块中，例如try/catch  ;synchronized等
Ctrl+E  #最近使用的文件
Ctrl+Shift+E  #最近更改的文件
Ctrl+P  #可以显示参数信息
Ctrl + O  #查看我们继承的类或者接口中的方法，以及我们要实现的方法
Ctrl + Alt + b  #查看接口实现类中方法
Ctrl+Shift+F  #在路径中查找
Ctrl+Shift+R  #在路径中替换
Ctrl+Alt+O  #优化导入的类和包
```
#### idea修改配置
Font(字体) Mononspaced；Size 18；Line Spacing 0.8；
#### bat
```bat
@echo off
echo "开始更新..  执行 git pull"
cd %~dp0
set currentFolder=%~dp0
for /D %%i in (Folder*) do ( 
  echo %%i
  cd %%i
  git pull
  rem git branch  字段rem是用来注释的
  cd ..
)
pause

if 1==1 (
  xcopy /y *.jar %currentFolder%jar  #bat拷贝命令参数/y是覆盖
  rd /q/s package  #删除目录package /q不询问，静默模式 /s目录树迭代删除
  md package  #创建目录package
  jar xf dev.jar  #静默解压dev.jar到当前目录
  pause  #暂停
)
```
```xml
<?xml version="1.0" encoding="UTF-8"?>

<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0 http://maven.apache.org/xsd/settings-1.0.0.xsd">
	<!-- localRepository | The path to the local repository maven will use to 
		store artifacts. | | Default: ${user.home}/.m2/repository <localRepository>/path/to/local/repo</localRepository> -->

	<localRepository>D:/path/maven-jar</localRepository>
  </settings>
  ```
