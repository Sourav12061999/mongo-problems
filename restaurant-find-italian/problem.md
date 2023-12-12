<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find documents in the `restaurants` collection where the `cuisine` field is equal to `Italian`.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
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
]
```

<h4 style="color:#397ce7">Sample Database:</h4>

```json
"restaurants":[
  {
    "address": {
      "building": "2780",
      "coord": [
        -73.98241999999999,
        40.579505
      ],
      "street": "Stillwell Avenue",
      "zipcode": "11224"
    },
    "borough": "Brooklyn",
    "cuisine": "American",
    "grades": [
      {
        "date": "2014-06-10T00:00:00.000Z",
        "grade": "A",
        "score": 5
      },
      {
        "date": "2013-06-05T00:00:00.000Z",
        "grade": "A",
        "score": 7
      },
      {
        "date": "2012-04-13T00:00:00.000Z",
        "grade": "A",
        "score": 12
      },
      {
        "date": "2011-10-12T00:00:00.000Z",
        "grade": "A",
        "score": 12
      }
    ],
    "name": "Riviera Caterer",
    "restaurant_id": "40356018"
  },
  {
    "address": {
      "building": "7114",
      "coord": [
        -73.9068506,
        40.6199034
      ],
      "street": "Avenue U",
      "zipcode": "11234"
    },
    "borough": "Brooklyn",  // can be any from  'Bronx', 'Brooklyn', 'Manhattan', 'Queens', 'Staten Island'
    "cuisine": "Delicatessen",
    "grades": [
      {
        "date": "2014-05-29T00:00:00.000Z",
        "grade": "A",
        "score": 10
      },
      {
        "date": "2014-01-14T00:00:00.000Z",
        "grade": "A",
        "score": 10
      },
      {
        "date": "2013-08-03T00:00:00.000Z",
        "grade": "A",
        "score": 8
      },
      {
        "date": "2012-07-18T00:00:00.000Z",
        "grade": "A",
        "score": 10
      },
      {
        "date": "2012-03-09T00:00:00.000Z",
        "grade": "A",
        "score": 13
      },
      {
        "date": "2011-10-14T00:00:00.000Z",
        "grade": "A",
        "score": 9
      }
    ],
    "name": "Wilken'S Fine Food",
    "restaurant_id": "40356483"
  }
]
```

```
cuisine can be
  'American',
  'Bagels/Pretzels',
  'Bakery',
  'Caribbean',
  'Chicken',
  'Chinese',
  'Continental',
  'Delicatessen',
  'Donuts',
  'French',
  'German',
  'Hamburgers',
  'Ice Cream, Gelato, Yogurt, Ices',
  'Irish',
  'Italian',
  'Jewish/Kosher',
  'Latin (Cuban, Dominican, Puerto Rican, South & Central American)',
  'Mexican',
  'Pizza',
  'Pizza/Italian',
  'Polish',
  'Sandwiches/Salads/Mixed Buffet',
  'Steak',
  'Turkish'
```
