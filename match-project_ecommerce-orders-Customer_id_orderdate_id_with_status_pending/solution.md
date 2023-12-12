<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([
  { $match: { status: "pending" }},{$project:{order_date:1,customer_id:1,_id:1}}
])

```
