### Query

1.

```json
db.restaurants.find({ "cuisine": { $ne: "American" }, "grades.grade": "A", "borough": { $ne: "Brooklyn" } }). sort({ "cuisine":
    -1 })
```

- Expected Output -

```
[
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee1"),
    address: {
      building: '60',
      coord: [ -74.0085357, 40.70620539999999 ],
      street: 'Wall Street',
      zipcode: '10005'
    },
    borough: 'Manhattan',
    cuisine: 'Turkish',
    grades: [
      { date: '2014-09-26T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-09-18T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-09-21T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2012-05-09T00:00:00.000Z', grade: 'A', score: 11 }
    ],
    name: 'The Country Cafe',
    restaurant_id: '40362715'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f0c"),
    address: {
      building: '845',
      coord: [ -73.965531, 40.765431 ],
      street: 'Lexington Avenue',
      zipcode: '10065'
    },
    borough: 'Manhattan',
    cuisine: 'Steak',
    grades: [
      { date: '2014-03-26T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-03-21T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-10-18T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2012-05-07T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2011-05-17T00:00:00.000Z', grade: 'A', score: 5 }
    ],
    name: "Donohue'S Steak House",
    restaurant_id: '40364572'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4eed"),
    address: {
      building: '405',
      coord: [ -73.97534999999999, 40.7516269 ],
      street: 'Lexington Avenue',
      zipcode: '10174'
    },
    borough: 'Manhattan',
    cuisine: 'Sandwiches/Salads/Mixed Buffet',
    grades: [
      { date: '2014-02-21T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-09-13T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2012-08-28T00:00:00.000Z', grade: 'A', score: 0 },
      { date: '2011-09-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-05-03T00:00:00.000Z', grade: 'A', score: 5 }
    ],
    name: 'Lexler Deli',
    restaurant_id: '40363426'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f15"),
    address: {
      building: '156-71',
      coord: [ -73.840437, 40.6627235 ],
      street: 'Crossbay Boulevard',
      zipcode: '11414'
    },
    borough: 'Queens',
    cuisine: 'Pizza/Italian',
    grades: [
      { date: '2014-10-29T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-10-30T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-06-12T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-03-27T00:00:00.000Z', grade: 'A', score: 9 }
    ],
    name: 'New Park Pizzeria & Restaurant',
    restaurant_id: '40364744'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef1"),
    address: {
      building: '464',
      coord: [ -73.9791458, 40.744328 ],
      street: '3 Avenue',
      zipcode: '10016'
    },
    borough: 'Manhattan',
    cuisine: 'Pizza',
    grades: [
      { date: '2014-08-05T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2014-03-06T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-07-09T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-01-30T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-01-05T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2011-09-26T00:00:00.000Z', grade: 'A', score: 0 }
    ],
    name: "Domino'S Pizza",
    restaurant_id: '40363644'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef2"),
    address: {
      building: '148',
      coord: [ -73.9806854, 40.7778589 ],
      street: 'West   72 Street',
      zipcode: '10023'
    },
    borough: 'Manhattan',
    cuisine: 'Pizza',
    grades: [
      { date: '2014-12-08T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2014-05-05T00:00:00.000Z', grade: 'B', score: 18 },
      { date: '2013-04-05T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-03-30T00:00:00.000Z', grade: 'A', score: 9 }
    ],
    name: "Domino'S Pizza",
    restaurant_id: '40363945'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f1e"),
    address: {
      building: '30-13',
      coord: [ -73.9151096, 40.763377 ],
      street: 'Steinway Street',
      zipcode: '11103'
    },
    borough: 'Queens',
    cuisine: 'Pizza',
    grades: [
      { date: '2014-10-06T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-10-10T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-10-24T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-06-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-01-17T00:00:00.000Z', grade: 'A', score: 10 }
    ],
    name: "Rizzo'S Fine Pizza",
    restaurant_id: '40364920'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f21"),
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
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f27"),
    address: {
      building: '103',
      coord: [ -74.001043, 40.729795 ],
      street: 'Macdougal Street',
      zipcode: '10012'
    },
    borough: 'Manhattan',
    cuisine: 'Mexican',
    grades: [
      { date: '2014-05-22T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-10-10T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-03-20T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-05-17T00:00:00.000Z', grade: 'B', score: 20 }
    ],
    name: "Panchito'S",
    restaurant_id: '40365348'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f12"),
    address: {
      building: '62',
      coord: [ -74.00310999999999, 40.7348888 ],
      street: 'Charles Street',
      zipcode: '10014'
    },
    borough: 'Manhattan',
    cuisine: 'Latin (Cuban, Dominican, Puerto Rican, South & Central American)',
    grades: [
      { date: '2014-05-02T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-05-20T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-05-24T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-01-18T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-10-03T00:00:00.000Z', grade: 'A', score: 10 }
    ],
    name: 'Seville Restaurant',
    restaurant_id: '40364439'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ec8"),
    address: {
      building: '2206',
      coord: [ -74.1377286, 40.6119572 ],
      street: 'Victory Boulevard',
      zipcode: '10314'
    },
    borough: 'Staten Island',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-10-06T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2014-05-20T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-04-04T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-01-24T00:00:00.000Z', grade: 'A', score: 9 }
    ],
    name: 'Kosher Island',
    restaurant_id: '40356442'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ecb"),
    address: {
      building: '97-22',
      coord: [ -73.8601152, 40.7311739 ],
      street: '63 Road',
      zipcode: '11374'
    },
    borough: 'Queens',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-11-24T00:00:00.000Z', grade: 'Z', score: 20 },
      { date: '2013-01-17T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-08-02T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-12-15T00:00:00.000Z', grade: 'B', score: 25 }
    ],
    name: 'Tov Kosher Kitchen',
    restaurant_id: '40356068'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f0a"),
    address: {
      building: '96-40',
      coord: [ -73.86137149999999, 40.7293762 ],
      street: 'Queens Boulevard',
      zipcode: '11374'
    },
    borough: 'Queens',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-03-13T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-09-30T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-04-26T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-09-11T00:00:00.000Z', grade: 'B', score: 24 },
      { date: '2011-09-19T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2011-03-17T00:00:00.000Z', grade: 'A', score: 12 }
    ],
    name: 'Ben-Best Deli & Restaurant',
    restaurant_id: '40364529'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f01"),
    address: {
      building: '1028',
      coord: [ -73.966032, 40.762832 ],
      street: '3 Avenue',
      zipcode: '10065'
    },
    borough: 'Manhattan',
    cuisine: 'Italian',
    grades: [
      { date: '2014-09-16T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2014-02-24T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-05-03T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-08-20T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-02-13T00:00:00.000Z', grade: 'A', score: 9 }
    ],
    name: 'Isle Of Capri Resturant',
    restaurant_id: '40364373'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f10"),
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
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f1b"),
    address: {
      building: '67',
      coord: [ -74.0707363, 40.59321569999999 ],
      street: 'Olympia Boulevard',
      zipcode: '10305'
    },
    borough: 'Staten Island',
    cuisine: 'Italian',
    grades: [
      { date: '2014-04-24T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2013-04-04T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2012-02-02T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2011-07-23T00:00:00.000Z', grade: 'A', score: 11 }
    ],
    name: 'Crystal Room',
    restaurant_id: '40365013'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f24"),
    address: {
      building: '93',
      coord: [ -73.99950489999999, 40.7169224 ],
      street: 'Baxter Street',
      zipcode: '10013'
    },
    borough: 'Manhattan',
    cuisine: 'Italian',
    grades: [
      { date: '2014-12-15T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-12-06T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-10-23T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-06-04T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-01-12T00:00:00.000Z', grade: 'A', score: 13 }
    ],
    name: 'Forlinis Restaurant',
    restaurant_id: '40365098'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f28"),
    address: {
      building: '146',
      coord: [ -73.9973041, 40.7188698 ],
      street: 'Mulberry Street',
      zipcode: '10013'
    },
    borough: 'Manhattan',
    cuisine: 'Italian',
    grades: [
      { date: '2014-05-02T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-03-14T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-09-26T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2012-02-15T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-09-15T00:00:00.000Z', grade: 'A', score: 11 }
    ],
    name: 'Angelo Of Mulberry St.',
    restaurant_id: '40365293'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ed5"),
    address: {
      building: '351',
      coord: [ -73.98513559999999, 40.7676919 ],
      street: 'West   57 Street',
      zipcode: '10019'
    },
    borough: 'Manhattan',
    cuisine: 'Irish',
    grades: [
      { date: '2014-09-06T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-07-22T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-07-31T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-12-29T00:00:00.000Z', grade: 'A', score: 12 }
    ],
    name: 'Dj Reynolds Pub And Restaurant',
    restaurant_id: '30191841'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f23"),
    address: {
      building: '15',
      coord: [ -73.9896713, 40.7287978 ],
      street: 'East    7 Street',
      zipcode: '10003'
    },
    borough: 'Manhattan',
    cuisine: 'Irish',
    grades: [
      { date: '2014-06-07T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2014-01-09T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-06-12T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-05-21T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-01-11T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-08-11T00:00:00.000Z', grade: 'B', score: 16 }
    ],
    name: "Mcsorley'S Old Ale House",
    restaurant_id: '40365075'
  }
]
```
