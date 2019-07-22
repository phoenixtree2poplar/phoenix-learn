#### https://blog.csdn.net/c5113620/article/category/7328319/1?  #java核心类学习
#### https://github.com/phoenixtree2poplar/my-git/blob/master/git-workflow-tutorial.md  #git工作流

```bash
call mvn -f pom.xml dependency:copy-dependencies  #根据pom.xml拉取仓库

git fetch --all   #强制拉取
git reset --hard origin/master  #强制覆盖本地
git rm -r --cached .gitignore  #刷新文件缓存

PURGE RECYCLEBIN  #清除回收BIN，gaussdb数据库命令

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

#### bat命令遍历当前目录并执行指定操作
```bash
@echo off
echo "开始更新..  执行 git pull"
cd %~dp0
set currentFolder=%~dp0
for /D %%i in (Folder*) do ( 
echo %%i
cd %%i
git pull
cd ..
)
pause
```
