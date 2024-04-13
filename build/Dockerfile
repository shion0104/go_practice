# goバージョン
FROM golang:1.22.1-alpine3.18
# アップデートとgitのインストール
RUN apk update && apk add git
# # go-practiceディレクトリの作成
RUN mkdir /go/src/github.com/go-practice
# # ワーキングディレクトリの設定
WORKDIR /go/src/github.com/go-practice
# # ホストのファイルをコンテナの作業ディレクトリに移行
ADD . /go/src/github.com/go-practice
# # パッケージのインポート
RUN go get -u golang.org/x/tools/cmd/goimports