<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.payments.aggregate([{$sort:{payment_date:-1}},{$limit:1},{$group:{_id:"$paymentMethod"}}])

```

result ==>

```json
[
  {
    "_id": "UPI"
  }
]
```
