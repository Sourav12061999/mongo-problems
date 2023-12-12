<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.buyers.aggregate([
  { $match: { "address.state": "CA" } },
  { $sort: { name: -1 } },
  { $limit: 3 }
])
```
