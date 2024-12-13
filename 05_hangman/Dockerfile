FROM golang:1.17

RUN go get -d github.com/TimothyDJones/pacgo-learn
WORKDIR /go/pkg/mod/github.com/\!timothy\!d\!jones/pacgo-learn\@v0.0.0-20191030221026-ca64f5338887

RUN go get -d https://github.com/Archilive/Hangman-Web
WORKDIR /go/pkg/mod/github.com/\!archilive/\!hangman-\!web/server

EXPOSE 8080

CMD go run main.go
