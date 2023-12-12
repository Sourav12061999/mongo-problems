### Queries

1.

```json
db.buyers.find({email: /@hotmail\.com$/}, {name: 1, email: 1, _id: 0})
```

2.

```json
db.buyers.aggregate([
  {$match:{email: /@hotmail\.com$/}},
  {$project:{name: 1, email: 1, _id: 0}}
  ])
```

--> result

```json
[
  {
    "name": "John Smith",
    "email": "john@hotmail.com"
  }
]
```
