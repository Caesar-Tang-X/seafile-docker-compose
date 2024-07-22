# SeaFile Docker Compose YML File


## 简介
    docker 一键启动 SeaFile 容器的 docker-compose.yml 配置


## 镜像环境：
	mariadb:10.11
	memcached:1.6.18
	seafileltd/seafile-mc:11.0.9


## 导入镜像：
	docker load -i 镜像包


## 启动命令：
	docker-compose up -d


## 安装及生成数据路径：
    ├── seafile 
        ├── images                      镜像文件文件目录
        ├── seafile                     容器挂载目录
            ├── db                      	数据库目录
                └── data                   		数据库数据录
            └── app                        	应用目录
                └── data                   		应用数据目录
        ├── docker-compose.yml          docker-compose.yml
        └── README.md                   README.md


## 隐私信息配置：
	1. 修改 SeaFile admin 账号的初始邮箱及密码, 文件路径：docker-compose.yml



