### Query

1.  db.restaurants.find( { "borough": { $in: ["Staten Island", "Queens", "Bronx", "Brooklyn"] } }, { "restaurant_id": 1, "name": 1,
    "borough": 1, "cuisine": 1 });

- Expected Output -

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d949591"),
    borough: 'Brooklyn',
    cuisine: 'American',
    name: 'Riviera Caterer',
    restaurant_id: '40356018'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949592"),
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    name: "Wilken'S Fine Food",
    restaurant_id: '40356483'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949593"),
    borough: 'Staten Island',
    cuisine: 'Jewish/Kosher',
    name: 'Kosher Island',
    restaurant_id: '40356442'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949594"),
    borough: 'Brooklyn',
    cuisine: 'Hamburgers',
    name: "Wendy'S",
    restaurant_id: '30112340'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949595"),
    borough: 'Bronx',
    cuisine: 'Bakery',
    name: 'Morris Park Bake Shop',
    restaurant_id: '30075445'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949596"),
    borough: 'Queens',
    cuisine: 'Jewish/Kosher',
    name: 'Tov Kosher Kitchen',
    restaurant_id: '40356068'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949597"),
    borough: 'Queens',
    cuisine: 'American',
    name: 'Brunos On The Boulevard',
    restaurant_id: '40356151'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949598"),
    borough: 'Brooklyn',
    cuisine: 'American',
    name: 'Regina Caterers',
    restaurant_id: '40356649'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949599"),
    borough: 'Brooklyn',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    name: 'Taste The Tropics Ice Cream',
    restaurant_id: '40356731'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959a"),
    borough: 'Bronx',
    cuisine: 'American',
    name: 'Wild Asia',
    restaurant_id: '40357217'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959b"),
    borough: 'Brooklyn',
    cuisine: 'American',
    name: 'C & C Catering Service',
    restaurant_id: '40357437'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959c"),
    borough: 'Brooklyn',
    cuisine: 'Jewish/Kosher',
    name: 'Seuda Foods',
    restaurant_id: '40360045'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959d"),
    borough: 'Brooklyn',
    cuisine: 'Chinese',
    name: 'May May Kitchen',
    restaurant_id: '40358429'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959f"),
    borough: 'Queens',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    name: 'Carvel Ice Cream',
    restaurant_id: '40361322'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a1"),
    borough: 'Brooklyn',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    name: 'Carvel Ice Cream',
    restaurant_id: '40360076'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a2"),
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    name: 'Nordic Delicacies',
    restaurant_id: '40361390'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a3"),
    borough: 'Brooklyn',
    cuisine: 'American',
    name: 'The Movable Feast',
    restaurant_id: '40361606'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a5"),
    borough: 'Queens',
    cuisine: 'Delicatessen',
    name: "Sal'S Deli",
    restaurant_id: '40361618'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a6"),
    borough: 'Queens',
    cuisine: 'Delicatessen',
    name: "Steve Chu'S Deli & Grocery",
    restaurant_id: '40361998'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495ab"),
    borough: 'Brooklyn',
    cuisine: 'Hamburgers',
    name: 'White Castle',
    restaurant_id: '40362344'
  }
]
```
