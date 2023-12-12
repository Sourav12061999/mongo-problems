<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Find all products that are not in category 1 or 2
- <span style="color:red">Hint:</span> - use `$nin`

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "_id": 7,
    "name": "Beats Studio Buds",
    "category_id": 3,
    "price": 149.99,
    "quantity": 50,
    "supplier_id": 6
  },
  {
    "_id": 8,
    "name": "Bose QuietComfort 35",
    "category_id": 3,
    "price": 249.99,
    "quantity": 50,
    "supplier_id": 7
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
