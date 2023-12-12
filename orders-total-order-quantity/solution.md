### Queries

1. db.pizza-orders.aggregate( [ 
   {
      $match: { size: "medium" }
   },
   {
      $group: { _id: "$name", totalQuantity: { $sum: "$quantity" } }
   }
] )

- Example output:

```
[
   { _id: 'Cheese', totalQuantity: 50 },
   { _id: 'Vegan', totalQuantity: 10 },
   { _id: 'Pepperoni', totalQuantity: 20 }
]
```
