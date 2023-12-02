FROM golang:latest
# Set the working directory inside the container
WORKDIR /app
#Copy the application source code from this go-app folder into the container
COPY go-app .

RUN make build

EXPOSE 8080

CMD ["./out/go-app"]
