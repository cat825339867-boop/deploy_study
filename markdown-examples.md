### 部署网站
1. 把项目提交到git上
2. 连接服务器

### ssh
ssh 账号@公网ip

### Linux
查看当前目录下文件 ls
查看隐藏文件 ls -a
切换目录 cd
创建目录 mkdir xxx
下载 apt install xxx
查看文件内容 cat xxx
获取当前目录路径 pwd  /home/web/deploy_study/.vitepress/dist
编辑文件 vim   编辑按下i键(insert)  保存并退出 :wq  不保存就直接:q


```sh
apt install git
apt install nginx
apt install nodejs
apt install npm
```

### nginx
nginx安装完成后默认安装在etc

```
        server{
          listen 81;
          server_name haha;

          location / {
            root /home/web/deploy_study/.vitepress/dist;
            index index.html;
           }
        }
```

启动nginx及重启
```
nginx
nginx -s reload
```
