###RESTful API for SFDC / Force.com Developer Project

_Thanks to [json-server](https://github.com/typicode/json-server)_ for making it so easy to setup.

```
GET    /opportunities
GET    /opportunities/1
POST   /opportunities
PUT    /opportunities/1
PATCH  /opportunities/1
DELETE /opportunities/1
```

```
GET /oopportunities?name=Wintheiser,%20Feil%20and%20Leffler
```

### Slice

Add `_start` and `_end` or `_limit` (an `X-Total-Count` header is included in the response)

```
GET /opportunities?_start=20&_end=30
GET /opportunities/1/opportunities?_start=20&_end=30
GET /opportunities/1/opportunities?_start=20&_limit=10
```

### Sort

Add `_sort` and `_order` (ascending order by default)

```
GET /opportunities?_sort=views&_order=DESC
GET /opportunities/1/opportunities?_sort=name&_order=ASC
```
