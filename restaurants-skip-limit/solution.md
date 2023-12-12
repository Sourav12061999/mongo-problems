### Query

1.  db.restaurants.find({"borough": "Bronx"}).skip(5).limit(5);

- Expected Output

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d9495c8"),
    address: {
      building: '658',
      coord: [ -73.81363999999999, 40.82941100000001 ],
      street: 'Clarence Ave',
      zipcode: '10465'
    },
    borough: 'Bronx',
    cuisine: 'American',
    grades: [
      { date: '2014-06-21T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2012-07-11T00:00:00.000Z', grade: 'A', score: 10 }
    ],
    name: 'Manhem Club',
    restaurant_id: '40364363'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495e5"),
    address: {
      building: '2222',
      coord: [ -73.84971759999999, 40.8304811 ],
      street: 'Haviland Avenue',
      zipcode: '10462'
    },
    borough: 'Bronx',
    cuisine: 'American',
    grades: [
      { date: '2014-12-18T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2014-05-01T00:00:00.000Z', grade: 'B', score: 17 },
      { date: '2013-03-14T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-09-20T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2012-02-08T00:00:00.000Z', grade: 'B', score: 19 }
    ],
    name: 'The New Starling Athletic Club Of The Bronx',
    restaurant_id: '40364956'
  }
]
```
