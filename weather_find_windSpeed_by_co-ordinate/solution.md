### Queries

1. db.data.aggregate([
  {$match:{"position.coordinates":[-76,26.4]}},
  {$project:{windspeed:"$wind.speed.rate",_id:0}}
  ])


--> result

```
{
  windspeed: 13
}

```
