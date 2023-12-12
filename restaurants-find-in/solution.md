### Query

1.

```json
db.restaurants.find({
  borough: "Bronx",
  cuisine: {
    $in: ["American", "Chinese"]
  }
})
```

- Expected Output -

```
[
  {
    _id: ObjectId("64758d35308eef6bfe3c4ecf"),
    address: {
      building: '2300',
      coord: [ -73.8786113, 40.8502883 ],
      street: 'Southern Boulevard',
      zipcode: '10460'
    },
    borough: 'Bronx',
    cuisine: 'American',
    grades: [
      { date: '2014-05-28T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-06-19T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-06-15T00:00:00.000Z', grade: 'A', score: 3 }
    ],
    name: 'Wild Asia',
    restaurant_id: '40357217'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee7"),
    address: {
      building: '1236',
      coord: [ -73.8893654, 40.81376179999999 ],
      street: '238 Spofford Ave',
      zipcode: '10474'
    },
    borough: 'Bronx',
    cuisine: 'Chinese',
    grades: [
      { date: '2013-12-30T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2013-01-08T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-06-12T00:00:00.000Z', grade: 'B', score: 15 }
    ],
    name: 'Happy Garden',
    restaurant_id: '40363289'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef8"),
    address: {
      building: '277',
      coord: [ -73.8941893, 40.8634684 ],
      street: 'East Kingsbridge Road',
      zipcode: '10458'
    },
    borough: 'Bronx',
    cuisine: 'Chinese',
    grades: [
      { date: '2014-03-03T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-09-26T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-03-19T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-08-29T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2011-08-17T00:00:00.000Z', grade: 'A', score: 13 }
    ],
    name: 'Happy Garden',
    restaurant_id: '40364296'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4efd"),
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
    _id: ObjectId("64758d35308eef6bfe3c4f1a"),
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
