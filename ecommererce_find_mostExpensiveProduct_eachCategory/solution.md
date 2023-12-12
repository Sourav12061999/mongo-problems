### Queries

1.

```json
db.products.aggregate([
{ $sort : { price: -1 } },
{ $group: { _id: '$category_id',name: { $first : "$name" }, maxPrice: { $first: '$price' } } }
])
```

--> result

```json
[
  {
    "_id": 1,
    "name": "MacBook Pro",
    "maxPrice": 1999.99
  },
  {
    "_id": 2,
    "name": "LG OLED 55" TV",
    "maxPrice": 1999.99
  },
  {
    "_id": 3,
    "name": "Bose QuietComfort 35",
    "maxPrice": 249.99
  }
]
```
