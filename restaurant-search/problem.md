<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to Perform a case-insensitive search for restaurants in the `restaurants` collection based on the `name` field.
- Search value - `kosher`

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
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
    _id: ObjectId("64758d35308eef6bfe3c4ef3"),
    address: {
      building: '1423',
      coord: [ -73.9615132, 40.6253268 ],
      street: 'Avenue J',
      zipcode: '11230'
    },
    borough: 'Brooklyn',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-12-19T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-12-05T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-12-06T00:00:00.000Z', grade: 'A', score: 9 }
    ],
    name: 'Kosher Bagel Hole',
    restaurant_id: '40364220'
  }
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
