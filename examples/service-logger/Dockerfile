FROM golang:1.8
WORKDIR /go/src/github.com/ilgooz/service-logger
RUN go get -v github.com/ilgooz/mesg-go/service && \
    go get -v github.com/ilgooz/mesg-go/service/servicetest && \
    go get -v github.com/stvp/assert
COPY . .
RUN go install -v ./...
RUN cd /go/bin
CMD ["cmd"]