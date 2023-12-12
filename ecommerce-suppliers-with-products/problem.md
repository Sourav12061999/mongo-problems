<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write Mongo query to retrieve suppliers with the highest number of products and productCount in `descending` order with limit of `5`.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "_id": 1,
    "name": "Apple",
    "city": "Cupertino",
    "phone": "1-800-275-2273",
    "products": [
      {
        "_id": 1,
        "name": "iPhone 13",
        "category_id": 1,
        "price": 999.99,
        "quantity": 50,
        "supplier_id": 1
      },
      {
        "_id": 5,
        "name": "MacBook Pro",
        "category_id": 1,
        "price": 1999.99,
        "quantity": 50,
        "supplier_id": 1
      }
    ],
    "productCount": 2
  },
  {
    "_id": 2,
    "name": "Samsung",
    "city": "Seoul",
    "phone": "82-2-2255-0114",
    "products": [
      {
        "_id": 2,
        "name": "Samsung Galaxy S21",
        "category_id": 1,
        "price": 899.99,
        "quantity": 30,
        "supplier_id": 2
      }
    ],
    "productCount": 1
  },
  {
    "_id": 4,
    "name": "LG",
    "city": "Seoul",
    "phone": "82-2-3777-1114",
    "products": [
      {
        "_id": 4,
        "name": "LG OLED 55\" TV",
        "category_id": 2,
        "price": 1999.99,
        "quantity": 50,
        "supplier_id": 4
      }
    ],
    "productCount": 1
  },
  {
    "_id": 5,
    "name": "Dell",
    "city": "Round Rock",
    "phone": "1-800-624-9897",
    "products": [
      {
        "_id": 6,
        "name": "Dell XPS 13",
        "category_id": 1,
        "price": 1299.99,
        "quantity": 50,
        "supplier_id": 5
      }
    ],
    "productCount": 1
  },
  {
    "_id": 3,
    "name": "Sony",
    "city": "Tokyo",
    "phone": "81-3-6748-2111",
    "products": [
      {
        "_id": 3,
        "name": "Sony Bravia 65\" TV",
        "category_id": 2,
        "price": 1499.99,
        "quantity": 60,
        "supplier_id": 3
      }
    ],
    "productCount": 1
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
