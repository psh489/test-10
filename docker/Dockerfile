FROM nginx:latest

# 1. 경로 수정: ./default.conf -> docker/default.conf
COPY ./docker/default.conf /etc/nginx/conf.d/default.conf

# 2. HTML 파일은 루트 기준이므로 그대로 둡니다
COPY ./html /usr/share/nginx/html

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]