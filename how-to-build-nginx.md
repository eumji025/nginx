# 使用Clion编译nginx
请参考我们编译redis的方式

这里需要修改的点
1.将auto里的configure移动到根目录下
2.启动时候指定配置文件路径

默认nginx的配置在/usr/local/nginx/conf下
这里是系统的目录存在权限的问题，这里我们建议通过
-c  $PROJECTDIR$/conf/nginx.conf自己配置


## nginx debug
1. update nginx.conf
>daemon off;<br>
>master_process off;

2.find  http  method to debug

link
https://blog.csdn.net/liaomin416100569/article/details/105127557/
