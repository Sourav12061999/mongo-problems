<h1 style="color:#397ce7">Solution Queries:</h1>

1. db.payments.find({ payment_date: { $ne: null } })

- Response:

```json
[
  {
    "_id": 1,
    "payment_date": "2022-03-01",
    "amount": 50.25,
    "orderdtl_id": 1,
    "paymentMethod": "UPI",
    "paymentstatus": "success"
  },
  {
    "_id": 2,
    "payment_date": "2022-03-15",
    "amount": 25.5,
    "orderdtl_id": 2,
    "paymentMethod": "Debit Card",
    "paymentstatus": "success"
  },
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
    "_id": 5,
    "payment_date": "2022-05-05",
    "amount": 75.0,
    "orderdtl_id": 5,
    "paymentMethod": "COD",
    "paymentstatus": null
  },
  {
    "_id": 6,
    "payment_date": "2022-05-15",
    "amount": 50.75,
    "orderdtl_id": 6,
    "paymentMethod": "UPI",
    "paymentstatus": "success"
  },
  {
    "_id": 7,
    "payment_date": "2022-06-01",
    "amount": 25.5,
    "orderdtl_id": 7,
    "paymentMethod": "net banking",
    "paymentstatus": "pending"
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
    "_id": 9,
    "payment_date": "2022-07-05",
    "amount": 125.5,
    "orderdtl_id": 9,
    "paymentMethod": "UPI",
    "paymentstatus": "success"
  },
  {
    "_id": 10,

    "payment_date": "2022-08-05",
    "amount": 75.25,
    "orderdtl_id": 10,
    "paymentMethod": "UPI",
    "paymentstatus": "success"
  }
]
```
