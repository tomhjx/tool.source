FROM golang:1.17.5-bullseye
RUN apt-get update && \ 
    apt-get upgrade && \
    apt-get install -y libpcap-dev && \
    mkdir $HOME/src && \
    cd $HOME/src && \
    git clone --branch v0.92.0 https://github.com/gohugoio/hugo.git && \
    cd hugo && \
    go install --tags extended && \
    echo $GOPATH && \
    echo $GOROOT && \
    ls -ahl $GOROOT/bin