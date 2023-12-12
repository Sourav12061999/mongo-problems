<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.suppliers.aggregate([{$group:{_id:"$city"}}])

```

result ==>

```json
[
  {
    "_id": "Culver City"
  }
]
```
