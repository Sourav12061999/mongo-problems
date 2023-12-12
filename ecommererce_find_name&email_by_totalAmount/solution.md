### Queries

1.

```json
db.buyers.aggregate([
   { $lookup: { from: 'orders', localField: '_id', foreignField: 'customer_id', as: 'orders' } },
   { $match: { 'orders.total': { $gt: 50 } } },
   { $project: { name: 1, email: 1 } }
  ])
```

--> result

```json
[
  {
    "_id": 1,
    "name": "John Smith",
    "email": "john@example.com"
  },
  {
    "_id": 2,
    "name": "Jane Doe",
    "email": "jane@example.com"
  },
  {
    "_id": 3,
    "name": "Bob Johnson",
    "email": "bob@example.com"
  },
  {
    "_id": 4,
    "name": "Alice Lee",
    "email": "alice@example.com"
  },
  {
    "_id": 5,
    "name": "Tom Wilson",
    "email": "tom@example.com"
  }
]
```
