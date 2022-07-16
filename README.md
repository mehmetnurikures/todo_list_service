# todo_list_service
It can used for building up a new todo list.

## Create the database & "items" table

```sh
sqlite3 todo.db < todo.sql
```

## Start the server

```sh
FLASK_APP=main flask run
```

## Open another terminal and send a HTTP request to create a new todo item

```sh
curl localhost:5000/item/new -X POST -H 'Content-Type: application/json' -d '{"item":"vance item 123"}'
```
