<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.buyers.aggregate([{$group:{_id:"$address.city"}}])

```

result ==>

```json
[
  {
    "_id": "Boston"
  },
  {
    "_id": "Chicago"
  }
]
```
