<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.payments.aggregate([
  { $match: { paymentMethod: { $ne: "UPI" } }}
])

```
