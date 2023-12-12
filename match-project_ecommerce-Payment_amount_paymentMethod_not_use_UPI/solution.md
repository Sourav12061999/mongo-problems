<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.payments.aggregate([
  { $match: { paymentMethod: { $ne: "UPI" } }},{$project:{amount:1,paymentMethod:1,_id:0}}
])

```
