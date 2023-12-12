### Query

1.

```json
db.restaurants.aggregate([ { $unwind: "$grades" }, { $group: { _id: { cuisine: "$cuisine", restaurant_id: "$restaurant_id" }, avgScore: { $avg: "$grades.score" } } }, { $sort: { "_id.cuisine": 1, avgScore: -1 } }, { $group: { _id: "$_id.cuisine", topRestaurants: { $push: { restaurant_id: "$_id.restaurant_id", avgScore: "$avgScore" } } } }, { $project: { _id: 0, cuisine: "$_id", topRestaurants: { $slice: ["$topRestaurants", 5] } } }])
```

- Expected Output -

```
[
  {
    cuisine: 'Continental',
    topRestaurants: [
      { restaurant_id: '40363630', avgScore: 15 },
      { restaurant_id: '40364691', avgScore: 12.2 }
    ]
  },
  {
    cuisine: 'Donuts',
    topRestaurants: [ { restaurant_id: '40363098', avgScore: 9.5 } ]
  },
  {
    cuisine: 'Pizza/Italian',
    topRestaurants: [ { restaurant_id: '40364744', avgScore: 10.25 } ]
  },
  {
    cuisine: 'Turkish',
    topRestaurants: [ { restaurant_id: '40362715', avgScore: 10.5 } ]
  },
  {
    cuisine: 'Chinese',
    topRestaurants: [
      { restaurant_id: '40358429', avgScore: 27.6 },
      { restaurant_id: '40363289', avgScore: 11 },
      { restaurant_id: '40364296', avgScore: 10.8 },
      { restaurant_id: '40363920', avgScore: 10 },
      { restaurant_id: '40362432', avgScore: 9.125 }
    ]
  },
  {
    cuisine: 'Chicken',
    topRestaurants: [
      { restaurant_id: '40364304', avgScore: 17.6 },
      { restaurant_id: '40362098', avgScore: 10.666666666666666 }
    ]
  },
  {
    cuisine: 'Bagels/Pretzels',
    topRestaurants: [ { restaurant_id: '40363565', avgScore: 19.166666666666668 } ]
  },
  {
    cuisine: 'Delicatessen',
    topRestaurants: [
      { restaurant_id: '40364299', avgScore: 15.6 },
      { restaurant_id: '40363333', avgScore: 12.833333333333334 },
      { restaurant_id: '40356483', avgScore: 10 },
      { restaurant_id: '40361618', avgScore: 9.5 },
      { restaurant_id: '40361708', avgScore: 9.25 }
    ]
  },
  {
    cuisine: 'Jewish/Kosher',
    topRestaurants: [
      { restaurant_id: '40356068', avgScore: 17.75 },
      { restaurant_id: '40364529', avgScore: 12.333333333333334 },
      { restaurant_id: '40360045', avgScore: 11.8 },
      { restaurant_id: '40356442', avgScore: 10.5 },
      { restaurant_id: '40364220', avgScore: 10 }
    ]
  },
  {
    cuisine: 'Irish',
    topRestaurants: [
      { restaurant_id: '40365075', avgScore: 10.666666666666666 },
      { restaurant_id: '30191841', avgScore: 9.25 },
      { restaurant_id: '40365239', avgScore: 6.25 }
    ]
  },
  {
    cuisine: 'Pizza',
    topRestaurants: [
      { restaurant_id: '40365280', avgScore: 21.5 },
      { restaurant_id: '40363945', avgScore: 13.25 },
      { restaurant_id: '40364920', avgScore: 9.2 },
      { restaurant_id: '40363644', avgScore: 5.333333333333333 }
    ]
  },
  {
    cuisine: 'Italian',
    topRestaurants: [
      { restaurant_id: '40364668', avgScore: 19 },
      { restaurant_id: '40365293', avgScore: 11.4 },
      { restaurant_id: '40365098', avgScore: 11 },
      { restaurant_id: '40365355', avgScore: 10.4 },
      { restaurant_id: '40364305', avgScore: 10.25 }
    ]
  },
  {
    cuisine: 'Polish',
    topRestaurants: [ { restaurant_id: '40364404', avgScore: 16.25 } ]
  },
  {
    cuisine: 'Caribbean',
    topRestaurants: [ { restaurant_id: '40362869', avgScore: 8 } ]
  },
  {
    cuisine: 'German',
    topRestaurants: [ { restaurant_id: '40364449', avgScore: 16.8 } ]
  },
  {
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    topRestaurants: [
      { restaurant_id: '40361322', avgScore: 10.666666666666666 },
      { restaurant_id: '40363093', avgScore: 9 },
      { restaurant_id: '40360076', avgScore: 8.6 },
      { restaurant_id: '40356731', avgScore: 8.25 },
      { restaurant_id: '40363834', avgScore: 6.333333333333333 }
    ]
  },
  {
    cuisine: 'French',
    topRestaurants: [
      { restaurant_id: '40364576', avgScore: 21.5 },
      { restaurant_id: '40365264', avgScore: 10.666666666666666 }
    ]
  },
  {
    cuisine: 'Steak',
    topRestaurants: [
      { restaurant_id: '40364335', avgScore: 10 },
      { restaurant_id: '40364572', avgScore: 7.4 }
    ]
  },
  {
    cuisine: 'Bakery',
    topRestaurants: [
      { restaurant_id: '40363151', avgScore: 8.2 },
      { restaurant_id: '30075445', avgScore: 8.2 }
    ]
  },
  {
    cuisine: 'Hamburgers',
    topRestaurants: [
      { restaurant_id: '30112340', avgScore: 13.75 },
      { restaurant_id: '40362344', avgScore: 6.25 }
    ]
  }
]
```
