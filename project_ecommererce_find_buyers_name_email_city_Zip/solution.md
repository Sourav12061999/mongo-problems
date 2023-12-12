### Queries

1.

```json
db.buyers.aggregate([
  {$project:{name:1,email:1,city:"$address.city",zip:"$address.zip", _id: 0}}
  ])
```

--> result

```json
[
  {
    "name": "Tom Wilson",
    "email": "tom@example.com",
    "city": "Boston",
    "zip": "02101"
  }
]
```
