# todo

## Installation

```bash
dep ensure
go install github.com/go-swagger/go-swagger/cmd/swagger
swagger generate server --target rest-server --name TodoList --spec rest-server/swagger.yml
dep ensure
go install ./rest-server/cmd/todo-list-server
todo-list-server --scheme http
```