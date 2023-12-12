<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.products.aggregate([
  {$project:{price:1,name:1,_id:0}}
])

```
