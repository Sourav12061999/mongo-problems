<h1 style="color:#397ce7">Solution Queries:</h1>

1. db.payments.find({}, { paymentMethod: 1 })

- Response:

```json
[
  {
    "_id": 1,
    "paymentMethod": "UPI"
  },
  {
    "_id": 2,
    "paymentMethod": "Debit Card"
  },
  {
    "_id": 3,
    "paymentMethod": "Cradit Card"
  },
  {
    "_id": 4,
    "paymentMethod": "UPI"
  },

  {
    "_id": 5,
    "paymentMethod": "COD"
  },
  {
    "_id": 6,
    "paymentMethod": "UPI"
  },
  {
    "_id": 7,
    "paymentMethod": "net banking"
  },
  {
    "_id": 8,
    "paymentMethod": "UPI"
  },
  {
    "_id": 9,
    "paymentMethod": "UPI"
  },
  {
    "_id": 10,

    "paymentMethod": "UPI"
  },
  {
    "_id": 11,
    "paymentMethod": "UPI"
  }
]
```
