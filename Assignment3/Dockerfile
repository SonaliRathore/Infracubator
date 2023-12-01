FROM golang AS build
WORKDIR /usr/app/src
COPY go-app .
RUN make build-linux

FROM alpine
COPY --from=build /usr/app/src/out/go-app .
EXPOSE 8080
CMD ["./go-app"]
