<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.suppliers.aggregate([
  {$match:{name: "Sony" }}, {$project:{city:1,phone:1,_id:0}}
  ])

```
