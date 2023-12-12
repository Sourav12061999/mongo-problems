<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.products.aggregate([
  {$match:{category_id:1}},{$project:{_id:0}}
])

```
