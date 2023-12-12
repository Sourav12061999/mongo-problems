<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.suppliers.aggregate([
  {$match:{city:"Tokyo"}},{$project:{name:1,_id:0}}
  ])

```
