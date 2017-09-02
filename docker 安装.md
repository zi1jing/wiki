## 镜像

docker pull registry.cn-hangzhou.aliyuncs.com/denverdino/tensorflow:1.2.1-py3---：安装镜像（imagename:version）

docker save -o "I:\imagename" tensorflow1.2：保存镜像tensorflow1.2到I:\imagename

docker load --input image所在路径：加载镜像

docker commit imageName/ID newImageName:保存镜像修改

docker ps：查看镜像列表

## 容器

docker run -it -p 8888:8888 --name=tensorflow1.2 registry.cn-hangzhou.aliyuncs.com/denverdino/tensorflow:1.2.1-py3 /run_jupyter.sh --allow-root:服务器端运行tensorflow

docker start tensorflow1.2:打开docker容器

docker exec -it tensorflow1.2（注：containerName/ID） /bin/bash:客户端运行tensorflow1.2

## 文件复制

docker cp containerName/ID:filepath newfilepath：把本地文件复制到本地

docker run  -v I:\work:/notebook  imgeName/ID：在指定镜像中把本地目录I:\work挂载到/notebook，并运行镜像

参考[ 基于Docker的TensorFlow机器学习框架搭建和实例源码解读](http://blog.csdn.net/dream_an/article/details/55520205)
