# flask-microservices
Example microservices stack using Flask and Kong

Part 1: Dựng Mock server sử dụng json-server

![microservices-part 1](docs/microservices-part1.png)

```bash
curl http://localhost:80/posts
curl http://localhost:80/posts/1
```

Kết quả trông như sau:

```bash
$ curl http://localhost:80/posts                                    [23:33:34]
[
  {
    "id": 1,
    "body": "foo"
  },
  {
    "id": 2,
    "body": "bar"
  }
]%
$ curl http://localhost:80/posts/1                                  [23:33:36]
{
  "id": 1,
  "body": "foo"
}%
```