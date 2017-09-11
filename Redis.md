远程服务连接：
```
$ Redis-cli -h 127.0.0.1 -p 6379
```

远程服务停止：
```
$ redis-cli -h 172.168.10.254 -p6379 shutdown
```
 
有权限控制时(加上-a 密码)：

```
redis-cli -h 127.0.0.1 -p 6379 -a 123456
```

见[文章](http://blog.csdn.net/vtopqx/article/details/46833215)
