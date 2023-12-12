### Queries

1.

```json
db.suppliers.aggregate([
  { $lookup: { from: "products", localField: "_id", foreignField: "supplier_id", as: "products" } },
  { $addFields: { productCount: { $size: "$products" } } },
  { $sort: { productCount: -1 } },
  { $limit: 5 }
])

```
