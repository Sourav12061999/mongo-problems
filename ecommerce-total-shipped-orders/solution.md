<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([
  { $match: { status: "shipped" } },
  { $count: "total_shipped_orders" }
])

```
