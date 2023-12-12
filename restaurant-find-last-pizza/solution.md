### Query

1.

```json
db.restaurants.find({ cuisine: "Pizza" }).sort({ _id: -1 }).limit(1)
```
