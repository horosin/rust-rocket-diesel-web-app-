# Sample Rust Web APP

Built with Rocket and Diesel.

Based on [this article][tutorial].

## Development

Start a dev db
```
docker-compose up
```

Run migrations
```
diesel migration run \
  --database-url postgresql://postgres:example@localhost:5432/postgres
```

Start the app, the port will be printed.
```
cargo watch -x run
```

## Utils

Print schema
```
diesel print-schema
```




[tutorial]: https://itnext.io/creating-a-rust-web-app-with-rocket-and-diesel-58f5f6cacd27