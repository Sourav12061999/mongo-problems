<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find the restaurants that achieved a score is more than `30` but less than `50`.
- Hint - use `$elemMatch`

<h4 style="color:#397ce7">Sample Output:</h4>

```json
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
