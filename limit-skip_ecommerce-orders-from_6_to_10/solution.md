<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([{$skip:5},{$limit:5}])

```

result ==>

```json
[
   {
  _id: 6,
  "customer_id": 3,
  order_date: '2022-05-15',
  ship_date: '2022-05-18',
  status: 'shipped',
  total: 50.75
},
...,
{
  _id: 10,
  customer_id: 5,
  order_date: '2022-08-01',
  ship_date: '2022-08-05',
  status: 'shipped',
  total: 75.25
}
]
```
