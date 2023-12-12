<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.buyers.aggregate([
  { $match: { "address.state": "CA", "address.city": { $in: ["Los Angeles", "San Francisco"] } } }
])

```
