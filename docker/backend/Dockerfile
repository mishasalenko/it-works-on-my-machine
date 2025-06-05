FROM golang:1.21

WORKDIR /backend

COPY go.mod go.sum ./
RUN go mod download

COPY . .

RUN go build -o golang-demo

CMD ["./golang-demo"]
