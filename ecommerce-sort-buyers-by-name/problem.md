<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write Mongo query to sort buyers by name in descending order.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
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
  },
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
  },
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
  },
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
  },
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
