# flask-microservices
Example microservices stack using Flask and Kong

Part 1: Dựng Mock server sử dụng json-server

![microservices-part 1](docs/microservices-part1.png)

```bash
curl http://localhost:8080/posts
curl http://localhost:8080/posts/1
curl http://localhost:8081/users
```

Kết quả trông như sau:

```bash
$ curl http://localhost:80/posts
[
  {
    "id": 1,
    "body": "foo"
  },
  {
    "id": 2,
    "body": "bar"
  }
]

$ curl http://localhost:80/posts/1
{
  "id": 1,
  "body": "foo"
}

$ curl http://localhost:8081/users
[
  {
    "id": 1,
    "name": "roy",
    "location": "india"
  },
  {
    "id": 2,
    "name": "sam",
    "location": "wales"
  }
]
```