### Queries

1. db.data.aggregate([
  {$match:{"position.coordinates":[-5.3,60.9]}},
  {$project:{"windDirection":"$wind.direction.angle",_id:0}}
  ])
  .map((e)=>e.windDirection%360 ===0 ? "N" :e.windDirection%360 <90 ? "NE" : e.windDirection%360 == 90 ? "E" : (e.windDirection%360>90 && e.windDirection%360<180) ? "SE": e.windDirection%360 === 180 ? "S" : (e.windDirection%360>180 && e.windDirection%360<270) ? "SW" : e.windDirection%360 == 270 ? "W":"NW")



--> result

```
'SW'

```