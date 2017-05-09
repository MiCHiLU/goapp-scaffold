# goapp-scaffold
A scaffold for Google App Engine Golang.

[![wercker status](https://app.wercker.com/status/01a88b7c9b69392341715dc7b9a234ba/m/master "wercker status")](https://app.wercker.com/project/byKey/01a88b7c9b69392341715dc7b9a234ba)

# clone repository

    $ cd `goapp env GOPATH`
    $ mkdir -p src/github.com/MiCHiLU
    $ cd src/github.com/MiCHiLU
    $ git clone --depth 1 https://github.com/MiCHiLU/goapp-scaffold.git
    $ cd goapp-scaffold

# dep

    $ go get -u github.com/golang/dep/...
    $ dep init
    $ dep ensure

# start server

    $ dev_appserver.py backend

# with swagger

Go to http://editor.swagger.io/ , then save to `swagger.yaml`.

Install go-swagger:

    $ go get -u github.com/go-swagger/go-swagger/cmd/swagger

Generate code:

    $ make restapi

Get swagger-ui:

    $ make swagger-ui

Open [swagger-ui](http://localhost:8080/swagger-ui/?url=http://localhost:8080/swagger.json).

    $ open "http://localhost:8080/swagger-ui/?url=http://localhost:8080/swagger.json"
