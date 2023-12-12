<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write Mongo query to retrieve all the orders details for supplier with `_id:1` ?
- <span style="color:red">Hint:</span> use MongoDB aggregation pipeline with `$match`, `$lookup`, `$project`, `$unwind`
- Can use javaScript methods to get the final output.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "_id": 1,
    "order_id": 1,
    "product_id": 1,
    "quantity": 1,
    "price": 999.99,
    "payment_id": 1,
    "shipper_id": 1
  },
  {
    "_id": 4,
    "order_id": 5,
    "product_id": 5,
    "quantity": 1,
    "price": 1999.99,
    "payment_id": 4,
    "shipper_id": 2
  },
  {
    "_id": 8,
    "order_id": 9,
    "product_id": 5,
    "quantity": 1,
    "price": 1999.99,
    "payment_id": 8,
    "shipper_id": 3
  }
]
```

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
},
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
],
"orders": [
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
"total": 75.0
},
{
"_id": 4,
"customer_id": 2,
"order_date": "2022-04-15",
"ship_date": null,
"status": "pending",
"total": 100.0
},
{
"_id": 5,
"customer_id": 2,
"order_date": "2022-05-01",
"ship_date": "2022-05-05",
"status": "shipped",
"total": 75.0
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
"total": 35.0
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
"total": 50.0
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
},
{
"_id": 2,
"name": "Samsung Galaxy S21",
"category_id": 1,
"price": 899.99,
"quantity": 30,
"supplier_id": 2
},
{
"_id": 3,
"name": "Sony Bravia 65\" TV",
"category_id": 2,
"price": 1499.99,
"quantity": 60,
"supplier_id": 3
},
{
"_id": 4,
"name": "LG OLED 55\" TV",
"category_id": 2,
"price": 1999.99,
"quantity": 50,
"supplier_id": 4
},
{
"_id": 5,
"name": "MacBook Pro",
"category_id": 1,
"price": 1999.99,
"quantity": 50,
"supplier_id": 1
},
{
"_id": 6,
"name": "Dell XPS 13",
"category_id": 1,
"price": 1299.99,
"quantity": 50,
"supplier_id": 5
},
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
],
"payments": [
{
"\_id": 1,
"payment_date": "2022-03-01",
"amount": 50.25,
"orderdtl_id": 1,
"paymentMethod": "UPI",
"paymentstatus": "success"
},
{
"\_id": 2,
"payment_date": "2022-03-15",
"amount": 25.5,
"orderdtl_id": 2,
"paymentMethod": "Debit Card",
"paymentstatus": "success"
},
{
"\_id": 3,
"payment_date": null,
"amount": null,
"orderdtl_id": 3,
"paymentMethod": "Cradit Card",
"paymentstatus": "success"
},
{
"\_id": 4,
"payment_date": null,
"amount": null,
"orderdtl_id": 4,
"paymentMethod": "UPI",
"paymentstatus": null
},

    {
      "_id": 5,
      "payment_date": "2022-05-05",
      "amount": 75.0,
      "orderdtl_id": 5,
      "paymentMethod": "COD",
      "paymentstatus": null
    },
    {
      "_id": 6,
      "payment_date": "2022-05-15",
      "amount": 50.75,
      "orderdtl_id": 6,
      "paymentMethod": "UPI",
      "paymentstatus": "success"
    },
    {
      "_id": 7,
      "payment_date": "2022-06-01",
      "amount": 25.5,
      "orderdtl_id": 7,
      "paymentMethod": "net banking",
      "paymentstatus": "pending"
    },
    {
      "_id": 8,
      "payment_date": null,
      "amount": null,
      "orderdtl_id": 8,
      "paymentMethod": "UPI",
      "paymentstatus": "success"
    },
    {
      "_id": 9,
      "payment_date": "2022-07-05",
      "amount": 125.5,
      "orderdtl_id": 9,
      "paymentMethod": "UPI",
      "paymentstatus": "success"
    },
    {
      "_id": 10,

      "payment_date": "2022-08-05",
      "amount": 75.25,
      "orderdtl_id": 10,
      "paymentMethod": "UPI",
      "paymentstatus": "success"
    },
    {
      "_id": 11,
      "payment_date": null,
      "amount": null,
      "orderdtl_id": 11,
      "paymentMethod": "UPI",
      "paymentstatus": "success"
    }

],
"categories": [
{ "_id": 1, "name": "Electronics" },
{ "_id": 2, "name": "TVs" },
{ "_id": 3, "name": "Headphones" }
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
},
{
"_id": 2,
"order_id": 2,
"product_id": 6,
"quantity": 2,
"price": 2599.98,
"payment_id": 2,
"shipper_id": 2
},
{
"_id": 3,
"order_id": 3,
"product_id": 2,
"quantity": 1,
"price": 899.99,
"payment_id": 3,
"shipper_id": 3
},
{
"_id": 4,
"order_id": 5,
"product_id": 5,
"quantity": 1,
"price": 1999.99,
"payment_id": 4,
"shipper_id": 2
},
{
"_id": 5,
"order_id": 6,
"product_id": 3,
"quantity": 1,
"price": 1499.99,
"payment_id": 5,
"shipper_id": 1
},
{
"_id": 6,
"order_id": 6,
"product_id": 8,
"quantity": 1,
"price": 249.99,
"payment_id": 6,
"shipper_id": 1
},
{
"_id": 7,
"order_id": 7,
"product_id": 2,
"quantity": 1,
"price": 899.99,
"payment_id": 7,
"shipper_id": 2
},
{
"_id": 8,
"order_id": 9,
"product_id": 5,
"quantity": 1,
"price": 1999.99,
"payment_id": 8,
"shipper_id": 3
},
{
"_id": 9,
"order_id": 9,
"product_id": 6,
"quantity": 1,
"price": 1299.99,
"payment_id": 9,
"shipper_id": 2
},
{
"_id": 10,
"order_id": 10,
"product_id": 7,
"quantity": 1,
"price": 149.99,
"payment_id": 10,
"shipper_id": 1
},
{
"_id": 11,
"order_id": 11,
"product_id": 4,
"quantity": 1,
"price": 1999.99,
"payment_id": 11,
"shipper_id": 1
}
],
"shippers": [
{ "_id": 1, "name": "UPS", "phone": "1-800-742-5877" },
{ "_id": 2, "name": "FedEx", "phone": "1-800-463-3339" },
{ "_id": 3, "name": "DHL", "phone": "1-800-225-5345" }
],

"suppliers": [
{
"_id": 1,
"name": "Apple",
"city": "Cupertino",
"phone": "1-800-275-2273"
},
{ "_id": 2, "name": "Samsung", "city": "Seoul", "phone": "82-2-2255-0114" },
{ "_id": 3, "name": "Sony", "city": "Tokyo", "phone": "81-3-6748-2111" },
{ "_id": 4, "name": "LG", "city": "Seoul", "phone": "82-2-3777-1114" },
{
"_id": 5,
"name": "Dell",
"city": "Round Rock",
"phone": "1-800-624-9897"
},
{
"_id": 6,
"name": "Beats",
"city": "Culver City",
"phone": "1-800-442-4000"
},
{
"_id": 7,
"name": "Bose",
"city": "Framingham",
"phone": "1-800-379-2073"
}
]
}

```

```
