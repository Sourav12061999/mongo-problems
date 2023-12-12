<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.products.aggregate([{$sort:{price:1}},{$limit:1}])


```

result ==>

```json
{
  "_id": 7,
  "name": "Beats Studio Buds",
  "category_id": 3,
  "price": 149.99,
  "quantity": 50,
  "supplier_id": 6
}
```
