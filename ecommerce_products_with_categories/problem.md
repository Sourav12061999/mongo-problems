<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a Mongo query to retrieve all products from the `products` collection along with their corresponding category information from the `categories` collection ?

- <span style="color:red">Hint:</span> - use MongoDB aggregation pipeline with [$lookup](https://www.mongodb.com/docs/manual/reference/operator/aggregation/lookup/)

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "_id": 1,
    "name": "iPhone 13",
    "category_id": 1,
    "price": 999.99,
    "quantity": 50,
    "supplier_id": 1,
    "category": [{ "_id": 1, "name": "Electronics" }]
  },
  {
    "_id": 2,
    "name": "Samsung Galaxy S21",
    "category_id": 1,
    "price": 899.99,
    "quantity": 30,
    "supplier_id": 2,
    "category": [{ "_id": 1, "name": "Electronics" }]
  },
  {
    "_id": 3,
    "name": "Sony Bravia 65\" TV",
    "category_id": 2,
    "price": 1499.99,
    "quantity": 60,
    "supplier_id": 3,
    "category": [{ "_id": 2, "name": "TVs" }]
  },
  {
    "_id": 4,
    "name": "LG OLED 55\" TV",
    "category_id": 2,
    "price": 1999.99,
    "quantity": 50,
    "supplier_id": 4,
    "category": [{ "_id": 2, "name": "TVs" }]
  },
  {
    "_id": 5,
    "name": "MacBook Pro",
    "category_id": 1,
    "price": 1999.99,
    "quantity": 50,
    "supplier_id": 1,
    "category": [{ "_id": 1, "name": "Electronics" }]
  },
  {
    "_id": 6,
    "name": "Dell XPS 13",
    "category_id": 1,
    "price": 1299.99,
    "quantity": 50,
    "supplier_id": 5,
    "category": [{ "_id": 1, "name": "Electronics" }]
  },
  {
    "_id": 7,
    "name": "Beats Studio Buds",
    "category_id": 3,
    "price": 149.99,
    "quantity": 50,
    "supplier_id": 6,
    "category": [{ "_id": 3, "name": "Headphones" }]
  },
  {
    "_id": 8,
    "name": "Bose QuietComfort 35",
    "category_id": 3,
    "price": 249.99,
    "quantity": 50,
    "supplier_id": 7,
    "category": [{ "_id": 3, "name": "Headphones" }]
  }
]
```
