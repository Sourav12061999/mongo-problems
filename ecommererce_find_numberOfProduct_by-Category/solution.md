### Queries

1.

```json
db.categories.aggregate([
  {$match:{name:"Electronics"}},
  {$lookup:{from:"products",localField:"_id",foreignField:"category_id",as:'orders'}},
  {$project:{orders:1}},
  {$unwind:"$orders"},
  {$count:"totalProduct"}
  ])
```

    --> result

```json
[
  {
    "totalProduct": 4
  }
]
```
