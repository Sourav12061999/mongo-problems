<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write Mongo query to retrieve `orders` sorted by order date in `ascending` order.

<h4 style="color:#397ce7">Sample Output:</h4>

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
    "_id": 3,
    "customer_id": 1,
    "order_date": "2022-04-01",
    "ship_date": null,
    "status": "pending",
    "total": 75
  },
  {
    "_id": 4,
    "customer_id": 2,
    "order_date": "2022-04-15",
    "ship_date": null,
    "status": "pending",
    "total": 100
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
    "_id": 8,
    "customer_id": 3,
    "order_date": "2022-06-15",
    "ship_date": null,
    "status": "pending",
    "total": 35
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
  },
  {
    "_id": 11,
    "customer_id": 5,
    "order_date": "2022-08-15",
    "ship_date": null,
    "status": "pending",
    "total": 50
  }
]
```

<h4 style="color:#397ce7">Sample Database:</h4>

```json
{
  "buyers": [
    {
      "_id": 1,
      "name": "John Smith",
      "email": "john@hotmail.com",
      "address": {
        "street": "123 Main St",
        "city": "New York",
        "state": "NY",
        "zip": "10001"
      }
    }
  ],
  "orders": [
    {
      "_id": 1,
      "customer_id": 1,
      "order_date": "2022-03-01",
      "ship_date": "2022-03-05",
      "status": "shipped"          // can be shipped or pending
      "total": 50.25
    }
  ],
  "products": [
    {
      "_id": 1,
      "name": "iPhone 13",
      "category_id": 1,
      "price": 999.99,
      "quantity": 50,
      "supplier_id": 1
    }
  ],
  "payments": [
    {
      "_id": 1,
      "payment_date": "2022-03-01",
      "amount": 50.25,
      "orderdtl_id": 1,
      "paymentMethod": "UPI",      // can be UPI, Debit Card, Cradit Card, COD or net banking
      "paymentstatus": "success"  // can be shipped, pending, or null
    }
  ],
  "categories": [
    {
      "_id": 1,
      "name": "Electronics"
    }
  ],
  "order_details": [
    {
      "_id": 1,
      "order_id": 1,
      "product_id": 1,
      "quantity": 1,
      "price": 999.99,
      "payment_id": 1,
      "shipper_id": 1
    }
  ],
  "shippers": [
    {
      "_id": 1,
      "name": "UPS",     // can be UPS , FedEx, or DHL
      "phone": "1-800-742-5877"
    }
  ],
  "suppliers": [
    {
      "_id": 1,
      "name": "Apple",
      "city": "Cupertino",
      "phone": "1-800-275-2273"
    }
  ]
}
```
