---
layout:       post
title:        "HUSTOJ 安装操作（基于DEEPIN操作系统）"
author:       "Andy"
header-style: text
catalog:      true
tags:
    - Hustoj
    - Deepin
    - Oj
---
#### 开始安装
>[官方文档](https://github.com/zhblue/hustoj/)

- 在deepin终端中输入
    ```
    wget http://dl.hustoj.com/install-deepin20+.sh
    sudo bash install-deepin20+.sh
    ```

- 安装完成后在本地浏览器打开127.0.0.1

- 注册用户名为admin即可拿到oj管理权限

#### 关于删除公告和下方二维码方法：

- 打开终端

- 输入
    ```
    sudo su
    ```
- 获得root权限
    ```
    cd /home/hustoj
    ```
- 进入网站文件夹
    ```
    grep -rn 欢迎关注
    ```
    查找关键字所在文件，也可替换使用其他关键字

- 在文件管理器中打开此文件删除相关代码并保存

- 刷新页面后即可发现二维码被删除