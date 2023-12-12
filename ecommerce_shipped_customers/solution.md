### Queries

1.

```json
db.orders.aggregate([
   {
   $match: { "status": "shipped" }
   },
   {
   $lookup: {
   from: "buyers",
   localField: "customer_id",
   foreignField: "_id",
   as: "customer"
   }
   }
   ])
```

- Result -

```json
[
  {
    "_id": 1,
    "customer_id": 1,
    "order_date": "2022-03-01",
    "ship_date": "2022-03-05",
    "status": "shipped",
    "total": 50.25,
    "customer": [
      {
        "_id": 1,
        "name": "John Smith",
        "email": "john@example.com",
        "address": {
          "street": "123 Main St",
          "city": "New York",
          "state": "NY",
          "zip": "10001"
        }
      }
    ]
  },
  {
    "_id": 2,
    "customer_id": 1,
    "order_date": "2022-03-15",
    "ship_date": "2022-03-18",
    "status": "shipped",
    "total": 25.5,
    "customer": [
      {
        "_id": 1,
        "name": "John Smith",
        "email": "john@example.com",
        "address": {
          "street": "123 Main St",
          "city": "New York",
          "state": "NY",
          "zip": "10001"
        }
      }
    ]
  },
  {
    "_id": 5,
    "customer_id": 2,
    "order_date": "2022-05-01",
    "ship_date": "2022-05-05",
    "status": "shipped",
    "total": 75,
    "customer": [
      {
        "_id": 2,
        "name": "Jane Doe",
        "email": "jane@example.com",
        "address": {
          "street": "456 Elm St",
          "city": "Los Angeles",
          "state": "CA",
          "zip": "90001"
        }
      }
    ]
  },
  {
    "_id": 6,
    "customer_id": 3,
    "order_date": "2022-05-15",
    "ship_date": "2022-05-18",
    "status": "shipped",
    "total": 50.75,
    "customer": [
      {
        "_id": 3,
        "name": "Bob Johnson",
        "email": "bob@example.com",
        "address": {
          "street": "789 Oak St",
          "city": "Chicago",
          "state": "IL",
          "zip": "60601"
        }
      }
    ]
  },
  {
    "_id": 7,
    "customer_id": 3,
    "order_date": "2022-06-01",
    "ship_date": "2022-06-05",
    "status": "shipped",
    "total": 25.5,
    "customer": [
      {
        "_id": 3,
        "name": "Bob Johnson",
        "email": "bob@example.com",
        "address": {
          "street": "789 Oak St",
          "city": "Chicago",
          "state": "IL",
          "zip": "60601"
        }
      }
    ]
  },
  {
    "_id": 9,
    "customer_id": 4,
    "order_date": "2022-07-01",
    "ship_date": "2022-07-05",
    "status": "shipped",
    "total": 125.5,
    "customer": [
      {
        "_id": 4,
        "name": "Alice Lee",
        "email": "alice@example.com",
        "address": {
          "street": "321 Pine St",
          "city": "San Francisco",
          "state": "CA",
          "zip": "94101"
        }
      }
    ]
  },
  {
    "_id": 10,
    "customer_id": 5,
    "order_date": "2022-08-01",
    "ship_date": "2022-08-05",
    "status": "shipped",
    "total": 75.25,
    "customer": [
      {
        "_id": 5,
        "name": "Tom Wilson",
        "email": "tom@example.com",
        "address": {
          "street": "654 Maple St",
          "city": "Boston",
          "state": "MA",
          "zip": "02101"
        }
      }
    ]
  }
]
```
