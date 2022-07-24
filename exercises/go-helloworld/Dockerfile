FROM golang 

LABEL maintainer="mahmoud shabban"

WORKDIR /go/src/app

# I could have used COPY
ADD . /go/src/app/

# I could have 2 RUN comands instead of &&
RUN go mod init && go build -o helloworld

EXPOSE 6111

CMD ["./helloworld"]