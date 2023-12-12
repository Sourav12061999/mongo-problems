### Query

1. db.restaurants.aggregate([{ $unwind: "$grades" },{ $group: { _id: "$name", avgScore: { $avg: "$grades.score"}}}])

- Expected Output -

```
[
  { _id: "Dunkin' Donuts", avgScore: 9.5 },
  { _id: 'Seuda Foods', avgScore: 11.8 },
  { _id: 'Carvel Ice Cream', avgScore: 8.6875 },
  { _id: 'Hot Bagels', avgScore: 19.166666666666668 },
  { _id: 'Nyac Main Dining Room', avgScore: 11.833333333333334 },
  { _id: 'Douglaston Club', avgScore: 12 },
  { _id: '21 Club', avgScore: 12 },
  { _id: 'Wild Asia', avgScore: 6 },
  { _id: 'Polish National Home', avgScore: 16.25 },
  { _id: 'South Shore Swimming Club', avgScore: 9.333333333333334 },
  { _id: 'Ho Mei Restaurant', avgScore: 9.125 },
  { _id: "Lorenzo & Maria'S", avgScore: 15 },
  { _id: 'Dining Room', avgScore: 12.2 },
  { _id: 'Seville Restaurant', avgScore: 10.4 },
  { _id: "Tony'S Deli", avgScore: 12.833333333333334 },
  { _id: 'Golden Pavillion', avgScore: 10 },
  { _id: 'Spoon Bread Catering', avgScore: 15.75 },
  { _id: 'Manhem Club', avgScore: 7.5 },
  { _id: 'Criminal Court Bldg Cafeteria', avgScore: 11.25 },
  { _id: 'Shell Lanes', avgScore: 15.6 }
]
```
