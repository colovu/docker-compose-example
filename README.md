# Docker-Compose

**约定**：

- 本例程库中相关Volume存储的默认目录为`/tmp/volumes`，可以将本目录中的`volumes`文件夹直接复制或软连接至`/tmp`目录，直接运行用例；实际生产环境，应根据实际需要配置相应的Volume路径。
- 如果不适用当前目录中`volumes`内的配置文件，大部分镜像可以正常运行（不启用个性化配置的镜像启动方式）。如果无法正常启动镜像，需要检查配置文件中是否使用了特殊的配置资源信息。如：IP、Volume等



## 说明

如果Docker-Compose配置文件在当前目录，并使用默认命名`docker-compose.yml`，则启动命令类似如下：

```shell
$ docker-compose up
```

如果没有使用默认命名，可以使用指定配置文件的方式运行：

```shell
$ docker-compose -f file-name.yml up
```



## Docker-Compose配置文件

### single

主要为各个应用的单机版本Docker-Compose配置文件，用于单机版本测试验证，或单应用的独立服务器部署。



### vcluster

主要为各个应用的单机虚拟集群部署，用于测试集群工作配置方式。



### cluster

主要为各个应用的集群部署配置文件。



## 参考

- [Docker-Compose官方文档](https://docs.docker.com/compose/reference/overview/)
- [Docker-Compose菜鸟教程](https://www.runoob.com/docker/docker-compose.html)



----

本文原始来源 [Endial Fang](https://github.com/endial) @ [Github.com](https://github.com) ([项目地址](https://github.com/endial/studylife.git))
