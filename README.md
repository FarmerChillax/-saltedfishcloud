# saltedfishcloud
Quick start  saltedfishcloud with docker

本文档描述生产环境配置，不同环境请按需切换到对应分支使用
1. 开发环境 - dev
2. 测试环境 - test
3. 预发布环境 - release
4. 生产环境 - 当前分支(main)

## docker 环境要求
已验证环境: `Docker Compose version v2.10.2`

## Quick start guide
1. 克隆本项目
```shell
$ git clone https://github.com/FarmerChillax/saltedfishcloud.git
```
2. 进入到项目根目录

```shell
$ cd saltedfishcloud
```

3. 执行以下命令
```shell
$ docker-compose up -d
```

## 关键环境变量描述

| 变量名              | Description                                             |
| :------------------ | :------------------------------------------------------ |
| DATA_PATH_HOST      | 宿主机上 MySQL Redis 数据卷存放的目录路径(暂不支持分离) |
| DATA_VOLUMES        | 宿主机上 存储卷 存放的目录路径                          |
| FRONTED_PORT        | 前端端口号                                              |
| REG_CODE            | 注册邀请码                                              |
| MYSQL_PORT          | MySQL 访问端口                                          |
| MYSQL_USERNAME      | MySQL 账号                                              |
| MYSQL_PASSWORD      | MySQL 密码                                              |
| MYSQL_ROOT_PASSWORD | MySQL 管理员密码                                        |
| REDIS_PORT          | Redis 端口                                              |