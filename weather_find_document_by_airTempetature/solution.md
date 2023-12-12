### Queries

1.db.data.aggregate([
  {$match:{"airTemperature.value":{$lt:9}}},
  {$count:"totalDocument"}
  ])


--> result

```
{
  totalDocument: 9
}

```
