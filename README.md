<!-- README.md is generated from README.ecr, do not edit -->

# GraphQL server benchmarks

Graphql server benchmarks in many languages. Pull requests welcome, please read [CONTRIBUTING.md](CONTRIBUTING.md)

All servers implement a simple schema:

```graphql
type Query {
  hello: String!
}
```

The returned string is always `world`.

The API is served over HTTP using a common web server and load tested using [bombardier](https://github.com/codesenberg/bombardier).

### Results

| Name                          | Language      | Server          | Latency avg      | Requests      |
| ----------------------------  | ------------- | --------------- | ---------------- | ------------- |
| [static-rust](https://actix.rs/) | Rust | Actix Web | 1.83ms | 110kps |
| [graphql-crystal](https://github.com/graphql-crystal/graphql) | Crystal | Kemal | 3.15ms | 63kps |
| [gqlgen](https://github.com/99designs/gqlgen) | Go | net/http | 4.29ms | 47kps |
| [async-graphql](https://github.com/async-graphql/async-graphql) | Rust | Actix Web | 4.56ms | 44kps |
| [Juniper](https://github.com/graphql-rust/juniper) | Rust | Actix Web | 5.44ms | 37kps |
| [Hot Chocolate](https://github.com/ChilliCream/hotchocolate) | C# | ASP.NET | 8.34ms | 24kps |
| [Mercurius](https://github.com/mercurius-js/mercurius) | Node.js | Fastify | 10.04ms | 20kps |
| [graphql-go](https://github.com/graphql-go/graphql) | Go | net/http | 11.10ms | 18kps |
| [GraphqlD](https://github.com/burner/graphqld) | D | Vibe.d | 11.22ms | 18kps |
| [graphql-yoga](https://github.com/dotansimha/graphql-yoga) | Node.js | http | 15.36ms | 13kps |
| [agoo](https://github.com/ohler55/agoo) | Ruby/C | agoo | 18.85ms | 11kps |
| [graphql-jit](https://github.com/zalando-incubator/graphql-jit) | Node.js | http | 22.56ms | 8.9kps |
| [Absinthe](https://github.com/absinthe-graphql/absinthe) | Elixir | Phoenix | 24.53ms | 8.1kps |
| [Hono](https://github.com/honojs/graphql-server) | Bun | HonoJS | 27.49ms | 7.2kps |
| [apollo](https://github.com/apollographql/apollo-server) | Node.js | Express | 33.27ms | 6.0kps |
| [graphql-ruby](https://github.com/rmosolgo/graphql-ruby) | Ruby | Puma | 44.89ms | 5.7kps |
| [graphql-js](https://github.com/graphql/graphql-js) | Node.js | http | 48.37ms | 4.1kps |
| [nim-graphql](https://github.com/status-im/nim-graphql) | Nim | Chronos | 55.30ms | 3.8kps |
| [Sangria](https://github.com/sangria-graphql/sangria) | Scala | Akka HTTP | 98.86ms | 2.0kps |
| [Graphene](https://github.com/graphql-python/graphene) | Python | gunicorn | 115.05ms | 1.7kps |
| [Strawberry](https://github.com/strawberry-graphql/strawberry) | Python | gunicorn | 117.31ms | 1.7kps |
