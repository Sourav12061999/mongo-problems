<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.shippers.aggregate([
  {$match:{phone: "1-800-742-5877" }}, {$project:{name:1,_id:0}}
  ])

```
