FROM registry.access.redhat.com/ubi9/go-toolset:1.22.5-1731639025

COPY . .
RUN go mod download

RUN go build -o ./main

ENV PORT 8081
EXPOSE 8081

CMD [ "./main" ]
