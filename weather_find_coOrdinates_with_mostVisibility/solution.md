### Queries

1. db.data.aggregate([
  {$sort:{"visibility.distance.value":-1}},
  {$limit:1},
  {$project:{"position.coordinates":1,_id:0}}
  ])


--> result

```
{
  position: {
    coordinates: [
      -47.9,
      47.6
    ]
  }
}

```
