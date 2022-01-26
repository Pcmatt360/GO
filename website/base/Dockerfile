FROM golang:latest

RUN git clone https://github.com/Pcmatt360/GO.git
WORKDIR GO/website/base
RUN go build -o bookings cmd/web/*.go
WORKDIR GO/website/base
RUN chmod 777 /go/GO/website/base/bookings

EXPOSE 8080

ENTRYPOINT ["/bin/bash", "-c","/go/GO/website/base/bookings"]