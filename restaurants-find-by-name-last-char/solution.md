### Query

1.  db.restaurants.find( { name: /ia$/ }, { "restaurant_id": 1, "name": 1, "borough": 1, "cuisine": 1 });

- Expected Output -

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d94959a"),
    borough: 'Bronx',
    cuisine: 'American',
    name: 'Wild Asia',
    restaurant_id: '40357217'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495d0"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Criminal Court Bldg Cafeteria',
    restaurant_id: '40364443'
  }
]
```
