<h1 style="color:#397ce7">Solution Queries:</h1>

1. db.payments.find({ payment_date: null });

- Response:

```json
[
  {
    "_id": 3,
    "payment_date": null,
    "amount": null,
    "orderdtl_id": 3,
    "paymentMethod": "Cradit Card",
    "paymentstatus": "success"
  },
  {
    "_id": 4,
    "payment_date": null,
    "amount": null,
    "orderdtl_id": 4,
    "paymentMethod": "UPI",
    "paymentstatus": null
  },
  {
    "_id": 8,
    "payment_date": null,
    "amount": null,
    "orderdtl_id": 8,
    "paymentMethod": "UPI",
    "paymentstatus": "success"
  },
  {
    "_id": 11,
    "payment_date": null,
    "amount": null,
    "orderdtl_id": 11,
    "paymentMethod": "UPI",
    "paymentstatus": "success"
  }
]
```
