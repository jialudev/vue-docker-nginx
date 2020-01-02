# vue-docker-nginx

> A Vue.js project

## 将vue项目配合nginx在docker中打包运行

## Build Setup

``` bash
# 打开docker

#下载docker中下载nginx
docker pull nginx

# 安装vue项目中的npm依赖
npm install

# 本地打包，生成dist文件
npm run build

# docker创建镜像
docker build -t vue-docker-nginx .

# 本地localhost:4000端口监听容器80容器启动docker
docker run -p 4000:8080 -d vue-docker-nginx

```

现在就可以在本机游览器查看在docker中启动的项目了。http://localhost:4000/ 

![Image](https://raw.githubusercontent.com/Mary5haw/vue-docker-nginx/master/img/img1.png)