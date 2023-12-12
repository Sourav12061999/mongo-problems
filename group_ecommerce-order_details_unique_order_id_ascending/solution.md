<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.order_details.aggregate([{$group:{_id:"$order_id"}},{$sort:{_id:1}}])


```

result ==>

```json
[
  {
    "_id": 1
  },
  {
    "_id": 2
  }
]
```
