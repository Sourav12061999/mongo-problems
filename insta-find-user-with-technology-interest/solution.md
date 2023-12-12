### Query

1.

```json
db.users.find({ interests: "technology" },{email:1})
```
2.

```json
db.users.aggregate([{$match:{ interests: "technology" }},{$project:{email:1}}])
```
