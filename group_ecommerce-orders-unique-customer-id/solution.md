<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([{$group:{_id:"$customer_id"}}])

```

result ==>

```json
{
    "_id": 1
  },
  {
    "_id": 2
  },
  {
    "_id": 3
  },
  {
    "_id": 4
  },
  {
    "_id": 5
  }
```
