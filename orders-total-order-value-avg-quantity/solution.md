### Queries

1. db.inventory.aggregate( [ { $unwind : "$sizes" } ] )

- Example output:

```
[
  { _id: 1, item: 'ABC1', sizes: 'S' },
  { _id: 1, item: 'ABC1', sizes: 'M' },
  { _id: 1, item: 'ABC1', sizes: 'L' }
]
```
