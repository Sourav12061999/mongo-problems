<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.products.aggregate([{$group:{_id:"$category_id"}}])


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
  }
```
