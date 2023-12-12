### Queries

1.

```json
db.buyers.aggregate([
  {$project:{city:"$address.city",zip:"$address.zip", _id: 0}}
  ])
```

--> result

```json
[
  {
    "city": "Boston",
    "zip": "02101"
  }
]
```
