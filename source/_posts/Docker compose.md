---
title: Docker compose
date: '2024-08-21 14:18:28'
updated: '2024-08-21 14:26:49'
categories:
  - Docker
---
# 更新某个应用
背景：一组应用 stop 重启，启动docker-complse.yml 某个初始化资源重复创建导致启动失败，需要注释掉这条语句。
解决方式：

1. 停止容器 docker-compose stop 应用名（别名）
2. 修改 docker-compose.yml 文件
3. 启动 docker-compose up 应用名 -d
