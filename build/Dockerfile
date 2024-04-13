# goバージョン
FROM golang:1.22.1-alpine3.18
# アップデートとgitのインストール
RUN apk update && apk add git
# # ワーキングディレクトリの設定
ADD . /go-practice
WORKDIR /go-practice
# # パッケージのインポート
RUN go install golang.org/x/tools/cmd/goimports@latest