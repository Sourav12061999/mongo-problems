### Queries

1. db.buyers.find({ _id: { $nin: db.orders.distinct("customer_id") } },{name:1,_id:0})

   --> result

```json
[
  { "name": "John Smith" },
  { "name": "Jane Doe" },
  { "name": "Bob Johnson" },
  { "name": "Alice Lee" },
  { "name": "Tom Wilson" }
]
```
