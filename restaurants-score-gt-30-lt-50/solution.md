### Query

1.  db.restaurants.find({grades : { $elemMatch:{"score":{$gt : 30 , $lt :50}}}});

- Expected Output

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d949597"),
    address: {
      building: '8825',
      coord: [ -73.8803827, 40.7643124 ],
      street: 'Astoria Boulevard',
      zipcode: '11369'
    },
    borough: 'Queens',
    cuisine: 'American',
    grades: [
      { date: '2014-11-15T00:00:00.000Z', grade: 'Z', score: 38 },
      { date: '2014-05-02T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-03-02T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-02-10T00:00:00.000Z', grade: 'A', score: 13 }
    ],
    name: 'Brunos On The Boulevard',
    restaurant_id: '40356151'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495c1"),
    address: {
      building: '0',
      coord: [ -84.2040813, 9.9986585 ],
      street: 'Guardia Airport Parking',
      zipcode: '11371'
    },
    borough: 'Queens',
    cuisine: 'American',
    grades: [
      { date: '2014-05-16T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-05-10T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-05-15T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-11-02T00:00:00.000Z', grade: 'C', score: 32 }
    ],
    name: 'Terminal Cafe/Yankee Clipper',
    restaurant_id: '40364262'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495c4"),
    address: {
      building: '203',
      coord: [ -74.15235919999999, 40.5563756 ],
      street: 'Giffords Lane',
      zipcode: '10308'
    },
    borough: 'Staten Island',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2015-01-05T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2014-09-11T00:00:00.000Z', grade: 'C', score: 39 },
      { date: '2014-03-20T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-01-24T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-05-23T00:00:00.000Z', grade: 'A', score: 10 }
    ],
    name: 'B & M Hot Bagel & Grocery',
    restaurant_id: '40364299'
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
    _id: ObjectId("6447c9678dfeb17a7d9495d2"),
    address: {
      building: '45',
      coord: [ -73.9891878, 40.7375638 ],
      street: 'East   18 Street',
      zipcode: '10003'
    },
    borough: 'Manhattan',
    cuisine: 'American',
    grades: [
      { date: '2014-10-08T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-10-10T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-04-24T00:00:00.000Z', grade: 'C', score: 36 },
      { date: '2012-01-09T00:00:00.000Z', grade: 'A', score: 9 }
    ],
    name: 'Old Town Bar & Restaurant',
    restaurant_id: '40364389'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495d4"),
    address: {
      building: '180',
      coord: [ -73.9788694, 40.7665961 ],
      street: 'Central Park South',
      zipcode: '10019'
    },
    borough: 'Manhattan',
    cuisine: 'American',
    grades: [
      { date: '2014-12-15T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2014-08-07T00:00:00.000Z', grade: 'C', score: 40 },
      { date: '2013-07-29T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2012-12-13T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-07-30T00:00:00.000Z', grade: 'C', score: 4 },
      { date: '2012-02-16T00:00:00.000Z', grade: 'A', score: 2 }
    ],
    name: 'Nyac Main Dining Room',
    restaurant_id: '40364467'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495da"),
    address: {
      building: '311',
      coord: [ -73.98621899999999, 40.763406 ],
      street: 'West   51 Street',
      zipcode: '10019'
    },
    borough: 'Manhattan',
    cuisine: 'French',
    grades: [
      { date: '2014-11-10T00:00:00.000Z', grade: 'B', score: 15 },
      { date: '2014-04-03T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2013-07-17T00:00:00.000Z', grade: 'C', score: 36 },
      { date: '2013-02-06T00:00:00.000Z', grade: 'B', score: 22 },
      { date: '2012-07-16T00:00:00.000Z', grade: 'C', score: 36 },
      { date: '2012-03-08T00:00:00.000Z', grade: 'C', score: 7 }
    ],
    name: 'Tout Va Bien',
    restaurant_id: '40364576'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495db"),
    address: {
      building: '251',
      coord: [ -73.9775552, 40.7432016 ],
      street: 'East   31 Street',
      zipcode: '10016'
    },
    borough: 'Manhattan',
    cuisine: 'Italian',
    grades: [
      { date: '2014-04-22T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2013-06-19T00:00:00.000Z', grade: 'C', score: 32 },
      { date: '2012-05-22T00:00:00.000Z', grade: 'A', score: 12 }
    ],
    name: 'Marchis Restaurant',
    restaurant_id: '40364668'
  }
]
```
