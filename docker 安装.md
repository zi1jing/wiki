docker pull registry.cn-hangzhou.aliyuncs.com/denverdino/tensorflow:1.2.1-py3---：安装镜像（imagename:version）

docker save -o "I:\imagename" tensorflow1.2：保存镜像tensorflow1.2到I:\imagename

docker ps：查看镜像列表

docker run -it -p 8888:8888 --name=tensorflow1.2 registry.cn-hangzhou.aliyuncs.com/denverdino/tensorflow:1.2.1-py3 /run_jupyter.sh --allow-root:服务器端运行tensorflow

docker start tensorflow1.2:打开docker容器

docker exec -it tensorflow1.2（注：image name） /bin/bash:客户端运行tensorflow1.2

参考[ 基于Docker的TensorFlow机器学习框架搭建和实例源码解读](http://blog.csdn.net/dream_an/article/details/55520205)
