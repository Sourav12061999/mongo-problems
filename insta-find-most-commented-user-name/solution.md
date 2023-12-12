### Query

1.

```json
db.posts.aggregate([
    {$group:{_id:"$userId","count":{$sum:1}}},
    {$sort:{count:-1}},
    {$limit:1},
    {$lookup:{from: "users",
       localField: "_id",
       foreignField: "_id",
       as: "userDtl"}},{$project :{_id:0,"name":"$userDtl.name"}},
    { $unwind: "$name" }])
```


