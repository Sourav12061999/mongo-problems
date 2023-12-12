### Queries

1.

```json
db.payments.aggregate([
  { $match: { paymentMethod: "UPI" } },{$project:{amount:1,_id:0}}
])
```

--> result

```json
[
  {
    "amount": 75.25
  }
]
```
