### Query

1.

```json
db.restaurants.find( { "cuisine": { $ne: "American " }, "grades.score": { $gt: 40 }, "address.coord": { $lt: -65.754168 } });
```

- Expected Output -

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d94959d"),
    address: {
      building: '1269',
      coord: [ -73.871194, 40.6730975 ],
      street: 'Sutter Avenue',
      zipcode: '11208'
    },
    borough: 'Brooklyn',
    cuisine: 'Chinese',
    grades: [
      { date: '2014-09-16T00:00:00.000Z', grade: 'B', score: 21 },
      { date: '2013-08-28T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2013-04-02T00:00:00.000Z', grade: 'C', score: 56 },
      { date: '2012-08-15T00:00:00.000Z', grade: 'B', score: 27 },
      { date: '2012-03-28T00:00:00.000Z', grade: 'B', score: 27 }
    ],
    name: 'May May Kitchen',
    restaurant_id: '40358429'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495ca"),
    address: {
      building: '94',
      coord: [ -74.0061936, 40.7092038 ],
      street: 'Fulton Street',
      zipcode: '10038'
    },
    borough: 'Manhattan',
    cuisine: 'Chicken',
    grades: [
      { date: '2015-01-06T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2014-07-15T00:00:00.000Z', grade: 'C', score: 48 },
      { date: '2013-05-02T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-09-24T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-04-19T00:00:00.000Z', grade: 'A', score: 7 }
    ],
    name: 'Texas Rotisserie',
    restaurant_id: '40364304'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495dc"),
    address: {
      building: '261',
      coord: [ -73.94839189999999, 40.7224876 ],
      street: 'Driggs Avenue',
      zipcode: '11222'
    },
    borough: 'Brooklyn',
    cuisine: 'Polish',
    grades: [
      { date: '2014-05-31T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-05-10T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2012-02-17T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2011-10-14T00:00:00.000Z', grade: 'C', score: 54 }
    ],
    name: 'Polish National Home',
    restaurant_id: '40364404'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495ec"),
    address: {
      building: '4035',
      coord: [ -73.9395182, 40.8422945 ],
      street: 'Broadway',
      zipcode: '10032'
    },
    borough: 'Manhattan',
    cuisine: 'Pizza',
    grades: [
      { date: '2014-02-10T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-02-04T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-01-04T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2011-09-15T00:00:00.000Z', grade: 'C', score: 60 }
    ],
    name: 'Como Pizza',
    restaurant_id: '40365280'
  }
]
```
