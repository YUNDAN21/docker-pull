# Github Actions
两种方法均是基于github actions，具体见docker_image_pusher和DockerTarBuilder

前者是将从github action下载的镜像推送到阿里云的镜像仓库https://cr.console.aliyun.com/

后者是将从github action下载的镜像上传到github自身服务器，然后下载下来离线镜像，最后使用`docker load`命令导入离线镜像，用上述两步代替docker pull

当然也可以采用镜像站的方法下载镜像
