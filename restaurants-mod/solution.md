### Query

1.

```json
db.restaurants.find( { "grades.score": { $mod: [7, 0] } }, { "restaurant_id": 1, "name": 1, "grades": 1 })
```

- Expected Output -

```
[
  {
    _id: ObjectId("64758d35308eef6bfe3c4ec6"),
    grades: [
      { date: '2014-06-10T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2013-06-05T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-04-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-10-12T00:00:00.000Z', grade: 'A', score: 12 }
    ],
    name: 'Riviera Caterer',
    restaurant_id: '40356018'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4eca"),
    grades: [
      { date: '2014-03-03T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-09-11T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2013-01-24T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2011-11-23T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-03-10T00:00:00.000Z', grade: 'B', score: 14 }
    ],
    name: 'Morris Park Bake Shop',
    restaurant_id: '30075445'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ecc"),
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
    _id: ObjectId("64758d35308eef6bfe3c4ed1"),
    grades: [
      { date: '2014-11-10T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-10-10T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-10-04T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-05-21T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-12-30T00:00:00.000Z', grade: 'B', score: 19 }
    ],
    name: 'Seuda Foods',
    restaurant_id: '40360045'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ed2"),
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
    _id: ObjectId("64758d35308eef6bfe3c4ed3"),
    grades: [
      { date: '2014-05-07T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-05-03T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-04-30T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2011-12-27T00:00:00.000Z', grade: 'A', score: 0 }
    ],
    name: '1 East 66Th Street Kitchen',
    restaurant_id: '40359480'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4eda"),
    grades: [
      { date: '2014-08-16T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-08-27T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2012-09-20T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2011-09-29T00:00:00.000Z', grade: 'A', score: 10 }
    ],
    name: "Sal'S Deli",
    restaurant_id: '40361618'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4edb"),
    grades: [
      { date: '2014-03-19T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-03-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-03-27T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2011-04-05T00:00:00.000Z', grade: 'A', score: 7 }
    ],
    name: "Steve Chu'S Deli & Grocery",
    restaurant_id: '40361998'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ede"),
    grades: [
      { date: '2014-09-15T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2014-03-04T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2013-07-18T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2013-01-09T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-04-10T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2011-11-15T00:00:00.000Z', grade: 'A', score: 7 }
    ],
    name: "Harriet'S Kitchen",
    restaurant_id: '40362098'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee0"),
    grades: [
      { date: '2014-03-18T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2013-03-18T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-10-10T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2011-09-22T00:00:00.000Z', grade: 'A', score: 2 }
    ],
    name: 'White Castle',
    restaurant_id: '40362344'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee2"),
    grades: [
      { date: '2014-05-13T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-05-08T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-09-22T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2011-06-06T00:00:00.000Z', grade: 'A', score: 12 }
    ],
    name: "Shashemene Int'L Restaura",
    restaurant_id: '40362869'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee3"),
    grades: [
      { date: '2014-04-21T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-11-12T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2013-06-04T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-11-14T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-10-11T00:00:00.000Z', grade: 'P', score: 0 },
      { date: '2012-05-24T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-12-08T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-07-20T00:00:00.000Z', grade: 'A', score: 11 }
    ],
    name: 'Ho Mei Restaurant',
    restaurant_id: '40362432'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee8"),
    grades: [
      { date: '2014-10-17T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-09-18T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2013-04-30T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-04-20T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2011-12-19T00:00:00.000Z', grade: 'A', score: 3 }
    ],
    name: "Olive'S",
    restaurant_id: '40363151'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4eed"),
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
    _id: ObjectId("64758d35308eef6bfe3c4ef0"),
    grades: [
      { date: '2014-02-25T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2013-08-14T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-08-07T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-03-26T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2011-11-04T00:00:00.000Z', grade: 'A', score: 0 },
      { date: '2011-06-29T00:00:00.000Z', grade: 'A', score: 4 }
    ],
    name: 'Snack Time Grill',
    restaurant_id: '40363590'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef1"),
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
    _id: ObjectId("64758d35308eef6bfe3c4ef4"),
    grades: [
      { date: '2014-06-02T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-12-27T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2013-03-18T00:00:00.000Z', grade: 'B', score: 26 },
      { date: '2012-02-01T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2011-07-06T00:00:00.000Z', grade: 'B', score: 25 }
    ],
    name: "Lorenzo & Maria'S",
    restaurant_id: '40363630'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef7"),
    grades: [
      { date: '2014-02-05T00:00:00.000Z', grade: 'A', score: 0 },
      { date: '2013-01-29T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2011-12-08T00:00:00.000Z', grade: 'A', score: 10 }
    ],
    name: "Sonny'S Heros",
    restaurant_id: '40363744'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4efa"),
    grades: [
      { date: '2014-11-18T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-11-07T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-04-24T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-03-20T00:00:00.000Z', grade: 'A', score: 5 }
    ],
    name: 'Plaza Bagels & Deli',
    restaurant_id: '40364286'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4efe"),
    grades: [
      { date: '2014-02-25T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-06-27T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-12-03T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2011-11-09T00:00:00.000Z', grade: 'A', score: 12 }
    ],
    name: 'Philadelhia Grille Express',
    restaurant_id: '40364305'
  }
]
```
