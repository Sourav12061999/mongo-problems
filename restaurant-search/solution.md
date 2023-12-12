### Query

1.

```json
db.restaurants.aggregate([
  { $match: { name: { $regex: "kosher", $options: "i" } } }
]);

```
