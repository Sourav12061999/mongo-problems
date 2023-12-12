<h1 style="color:#397ce7">Solution Queries:</h1>

1. db.payments.find({ paymentstatus: { $in: [null, "pending"] } })

- Response:

```json
[
  {
    "_id": 4,
    "payment_date": null,
    "amount": null,
    "orderdtl_id": 4,
    "paymentMethod": "UPI",
    "paymentstatus": null
  },
  {
    "_id": 5,
    "payment_date": "2022-05-05",
    "amount": 75,
    "orderdtl_id": 5,
    "paymentMethod": "COD",
    "paymentstatus": null
  },
  {
    "_id": 7,
    "payment_date": "2022-06-01",
    "amount": 25.5,
    "orderdtl_id": 7,
    "paymentMethod": "net banking",
    "paymentstatus": "pending"
  }
]
```
