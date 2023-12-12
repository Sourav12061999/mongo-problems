### Queries

1. db.orders.find({ship_date: {$ne: null}})

- Result -

```json
[
  {
    "_id": 1,
    "customer_id": 1,
    "order_date": "2022-03-01",
    "ship_date": "2022-03-05",
    "status": "shipped",
    "total": 50.25
  },
  {
    "_id": 2,
    "customer_id": 1,
    "order_date": "2022-03-15",
    "ship_date": "2022-03-18",
    "status": "shipped",
    "total": 25.5
  },
  {
    "_id": 5,
    "customer_id": 2,
    "order_date": "2022-05-01",
    "ship_date": "2022-05-05",
    "status": "shipped",
    "total": 75
  },
  {
    "_id": 6,
    "customer_id": 3,
    "order_date": "2022-05-15",
    "ship_date": "2022-05-18",
    "status": "shipped",
    "total": 50.75
  },
  {
    "_id": 7,
    "customer_id": 3,
    "order_date": "2022-06-01",
    "ship_date": "2022-06-05",
    "status": "shipped",
    "total": 25.5
  },
  {
    "_id": 9,
    "customer_id": 4,
    "order_date": "2022-07-01",
    "ship_date": "2022-07-05",
    "status": "shipped",
    "total": 125.5
  },
  {
    "_id": 10,
    "customer_id": 5,
    "order_date": "2022-08-01",
    "ship_date": "2022-08-05",
    "status": "shipped",
    "total": 75.25
  }
]
```
