### Queries

1.

```json
db.buyers.aggregate([{$match:{"address.state":"CA"}},{$project:{name: 1,_id:0}}])
```

--> result

```json
[
  {
    "name": "Jane Doe"
  },
  {
    "name": "Alice Lee"
  }
]
```
