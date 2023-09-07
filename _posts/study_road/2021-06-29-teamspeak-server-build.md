---
layout:       post
title:        "teamspeak 服务端（linux）安装教程"
author:       "Andy"
header-style: text
catalog:      true
tags:
    - Linux
    - Teamspeak
---
- 安装流程

    - 登录ts官网：www.teamspeak.com下载64位linux下服务端（需翻墙）

    - 将文件上传至服务器root目录下

    - 开放ts服务端所需要使用的端口：9987、10011、30033

    - 创建teamspeak用户并设置密码:
        ```
        useradd teamspeak
        passwd teamspeak
        ```
    - 解压上传的服务端文件压缩包：
        ```
        tar -xvf teamspeak3-server_linux_amd64-3.13.6.tar.bz2（版本号具体根据所使用的服务端更改）
        ```
    - 将解压后的文件放到指定文件夹：
        ```
        mv teamspeak3-server_linux_amd64 teamspeak3
        ```
    - 给teamspeak赋权（ts服务不允许使用root用户启动）：
        ```
        cp -R teamspeak3 /home/teamspeak
        chown -R teamspeak:teamspeak /home/teamspeak/teamspeak3
        ```
    - 切换至teamspeak用户启动ts服务：
        ```
        su - teamspeak
        cd teamspeak3
        touch .ts3server_license_accepted      \\同意ts的相关协议
        ./ts3server_startscript.sh start
        ```
    - 复制启动成功后出现的token秘钥，客户端登录服务器地址，首次登录会提醒输入秘钥即刚刚获取的token获得服务器管理权限

    - 开始享用自己的ts服务器与基友开黑