<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.payments.aggregate([
  { $match: { amount: {$gt:100} }},{$project:{paymentstatus:1,_id:0}}
])

```
