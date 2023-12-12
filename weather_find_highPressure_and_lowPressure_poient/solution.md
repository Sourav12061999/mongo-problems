### Queries

1. db.data.aggregate([
  sort:{"pressure.value":-1}},
  {$project:{"coordinates":"$position.coordinates","pressure":"$pressure.value",_id:0}}
  ])
  .toArray()
  .filter((e,i)=>i ==0 || i==14)


--> result

```
[
  {
    coordinates: [ 116.2, 6.8 ],
    pressure: 9999.9
  },
  {
    coordinates: [ 151.5, -1.1 ],
    pressure: 1006.4
  }
]

```
