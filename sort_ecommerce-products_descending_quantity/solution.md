<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.products.aggregate([{$sort:{quantity:-1}}])

```

result ==>

```json
[
  {
    "_id": 6,
    "name": "Dell XPS 13",
    "category_id": 1,
    "price": 1299.99,
    "quantity": 50,
    "supplier_id": 5
  },
  {
    "_id": 2,
    "name": "Samsung Galaxy S21",
    "category_id": 1,
    "price": 899.99,
    "quantity": 30,
    "supplier_id": 2
  }
]
```
