### Queries

1.

```json
db.buyers.aggregate([
  {$match:{email: /@hotmail\.com$/}},
  {$project:{city:"$address.city", _id: 0}}
  ])
```

--> result

```json
[
  {
    "city": "New York"
  }
]
```
