### Queries

1.  db.products.aggregate([
   {
     $group: {
       _id: "$category",
       totalCount: { $sum: 1 }
     }
   }
 ])


- Result -

```
[
  { _id: 'electronics', totalCount: 6 },
  { _id: "men's clothing", totalCount: 4 },
  { _id: 'jewelery', totalCount: 4 },
  { _id: "women's clothing", totalCount: 6 }
]

```

