### Query

1.

```json
db.restaurants.find({ name: { $regex: "Pizza", $options: "i" } })
```
