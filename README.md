## 热加载，背景图片，lombok，jetty
#### https://blog.csdn.net/c5113620/article/category/7328319/1?  #java核心类学习
#### https://blog.csdn.net/HeatDeath/article/details/80156993  #idea插件
#### https://blog.csdn.net/win7system/article/details/83508313  #idea插件
#### 想要把IDEA窗口拖拽回当前屏幕，可以找到项目中.idea文件夹下的workspace.xml文件全文搜索ProjectFrameBounds关键字，修改x的值为0或者直接将name=“x”的这一行删除即可，然后重启IDEA即可
```cmd
远程调试
java -Xdebug -agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=20001 -Dfile.encoding=utf-8 -jar poplar.jar --server.port=20000
```
