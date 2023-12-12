### Queries

1.

```json
db.suppliers.aggregate([
  {
    $group: {
      _id: "$city",
      count: { $sum: 1 }
    }
  },
  {
    $sort: { count: -1 }
  }
])

```
