<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.payments.aggregate([{$group:{_id:"$paymentstatus"}}])

```

result ==>

```json
[
  {
    "_id": "success"
  },
  {
    "_id": "pending"
  },
  {
    "_id": null
  }
]
```
