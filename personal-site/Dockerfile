# 使用轻量nginx镜像托管静态网页
FROM nginx:alpine
# 复制本地网页到容器nginx目录
COPY . /usr/share/nginx/html
# 对外暴露80端口
EXPOSE 80