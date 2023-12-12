<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.products.aggregate([{$sort:{price:-1}},{$limit:1}])


```

result ==>

```json
{
  "_id": 5,
  "name": "MacBook Pro",
  "category_id": 1,
  "price": 1999.99,
  "quantity": 50,
  "supplier_id": 1
}
```
