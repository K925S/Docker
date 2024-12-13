# 1. Go 1.16 이미지를 사용
FROM golang:1.16

# 2. 패키지를 다운로드할 Go 프로젝트를 설정
WORKDIR /app

# 3. Git 리포지토리 클론 (예: simplepacman)
RUN go get -d github.com/TimothyDJones/pacgo-learn

# 4. 8080 포트를 컨테이너에서 열기
EXPOSE 8080

# 5. 애플리케이션 실행
CMD ["go", "run", "main.go"]

