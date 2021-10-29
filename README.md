# simple-rocket-server

Kind of a todoAPI server. Just basic implementation which let you keeps data in sqlite db. Based on [this tutorial](https://www.youtube.com/watch?v=8RA6LSjXvRk).

### Routes:

- `GET /todo` - get all todos from the db
- `POST /todo ` + `{"message"}` - add the todo item to the db.
- `DELETE /todo/{id}` - delete todo with a given id.

### Testing

If you wish to test it, there you got a couple of commands that may help you with that:

#### Get all todo items:

`curl localhost:8000/todo`

#### Create todo item:

`curl local host:8000/todo -X POST -d '"todo stuff"' -H "Content-Type: application/json"`

#### Delete todo with a given id:

Here it's deleting the id = 1
`curl localhost:8000/todo/1 -X DELETE`
