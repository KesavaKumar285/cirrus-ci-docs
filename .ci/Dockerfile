FROM golang as liche
RUN CGO_ENABLED=0 GOOS=linux go get /go/src/github.com/raviqqe/liche

FROM squidfunk/mkdocs-material:latest
COPY --from=liche /go/bin/liche /bin/liche
