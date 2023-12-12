<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.testec.aggregate([
  {$match:{age:{$lt:30}}}, {$project:{name:1,_id:0,"city":"$address.city"}}
  ])

```
