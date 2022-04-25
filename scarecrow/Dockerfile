FROM golang

CMD apt update && \
    apt install -y openssl osslsigncode mingw-w64 && \
    git clone https://github.com/optiv/ScareCrow.git /ScareCrow

WORKDIR /ScareCrow

CMD go get github.com/fatih/color && \
    go get github.com/yeka/zip && \
    go get github.com/josephspurrier/goversioninfo && \
    go build ScareCrow.go

WORKDIR /data

ENTRYPOINT [/ScareCrow/ScareCrow]
