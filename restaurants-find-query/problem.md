<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find the restaurants which do not prepare any cuisine of `American` and achieved a grade point `A` not belongs to the borough `Brooklyn`.
- The document must be displayed according to the cuisine in descending order.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
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
