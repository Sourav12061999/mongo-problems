<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find the restaurants who achieved a score more than `50`.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    _id: ObjectId("64758d35308eef6bfe3c4ed2"),
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
    _id: ObjectId("64758d35308eef6bfe3c4f11"),
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

```text
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
