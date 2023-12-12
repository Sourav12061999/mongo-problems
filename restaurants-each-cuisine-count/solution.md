### Query

1. db.restaurants.aggregate([{ $group: { _id: "$cuisine", count: { $sum: 1 } } }])

- Expected Output -

```
[
  { _id: 'Irish', count: 3 },
  { _id: 'Italian', count: 7 },
  { _id: 'German', count: 1 },
  { _id: 'Caribbean', count: 1 },
  { _id: 'French', count: 2 },
  { _id: 'Chicken', count: 2 },
  { _id: 'American', count: 40 },
  { _id: 'Bagels/Pretzels', count: 1 },
  { _id: 'Polish', count: 1 },
  { _id: 'Pizza/Italian', count: 1 },
  { _id: 'Hamburgers', count: 2 },
  { _id: 'Bakery', count: 2 },
  { _id: 'Ice Cream, Gelato, Yogurt, Ices', count: 5 },
  { _id: 'Delicatessen', count: 9 },
  { _id: 'Chinese', count: 5 },
  { _id: 'Mexican', count: 1 },
  { _id: 'Sandwiches/Salads/Mixed Buffet', count: 1 },
  { _id: 'Steak', count: 2 },
  { _id: 'Pizza', count: 4 },
  { _id: 'Continental', count: 2 }
]
```
