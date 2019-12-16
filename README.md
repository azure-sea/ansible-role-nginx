Ansible Role: Nginx
=========
在RedHat/CentOS上安装Nginx的Ansible角色 \
An Ansible Role that installs Nginx on RedHat/CentOS


Requirements
------------

无。\
 None.

Role Variables
--------------
下面介绍了可用变量和默认值(可参照"vars/main.yml"文件)
The following describes the available variables and default values(refer to the "vars/main.yml" file)

1. Nginx 版本信息。\
  Nginx Version Information  

```
nginx_version: 1.16.1
```
下面是默认的一些编译安装的一些默认变量(可参照"dafaults/main.yml"文件) \
Here are some default variables for compiling and installing(refer to the "defaults/main.yml" file)

2. Nginx 安装目录。\
 Nginx installation directory.

```
nginx_dir: /work/oldsoft
```
3. Nginx 软链接目录。\
 Nginx soft link directory.


```
nginx_link_dir: /work/nginx
```
4. Nginx 运行用户和组。\
 Nginx running users and groups.

```
nginx_run_user: nginx
nginx_run_group: nginx
```

Dependencies
------------
无依赖。\
None.

Example Playbook
----------------
```
- hosts: servers
  roles:
    - { role: nginx }
```
License
-------

BSD

Author Information
------------------
Author: Azure-sea \
QQ: 2053921233 \
email: 2053921233@qq.com
