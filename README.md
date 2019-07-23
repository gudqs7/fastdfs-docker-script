# fastdfs-docker-script
使用docker + docker-compose 一键弄个 fastdfs 吧

```
vi nginx.conf #没啥可编辑的
vi storage.conf #也没啥可改的
vi tracker.conf #不存在这个文件, 想改自己修改一下 yml 文件

#起飞
docker-compose up -d

docker exec -it storage /bin/bash
```
cd /fdfs_conf
fdfs_upload_file storage.conf anti-steal.jpg #上传一个图片吧, 返回路径如 /group1/M00/00/00/xxxx  
# 访问 localhost:8088/group1/M00/00/00/xxxx 吧
```
```
