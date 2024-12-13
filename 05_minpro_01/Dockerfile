# 1. 베이스 이미지를 설정 (Nginx)
FROM nginx:alpine

# 2. Git 설치
RUN apk add --no-cache git

# 3. 리포지토리를 클론할 위치 설정
WORKDIR /usr/share/nginx/html

# 4. Git을 설치하고 리포지토리 클론
RUN git clone https://github.com/RishabhDevbanshi/Pacman-Game.git
RUN rm -rf .git

# 5. Nginx 서비스 포트 8080 설정
EXPOSE 8080

# 6. Nginx 실행
CMD ["nginx", "-g", "daemon off;"]
