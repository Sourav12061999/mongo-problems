<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find the restaurants that have more than 5 grades (see in sample output - gradeCount) and sort them by the number of grades in `descending` order.
- Limit the number of results to `10`

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee3"),
    address: {
      building: '103-05',
      coord: [ -73.8642349, 40.75356 ],
      street: '37 Avenue',
      zipcode: '11368'
    },
    borough: 'Queens',
    cuisine: 'Chinese',
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
    restaurant_id: '40362432',
    gradeCount: 8
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4eea"),
    address: {
      building: '1069',
      coord: [ -73.902463, 40.694924 ],
      street: 'Wyckoff Avenue',
      zipcode: '11385'
    },
    borough: 'Queens',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-05-08T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-12-12T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2013-06-21T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-12-24T00:00:00.000Z', grade: 'B', score: 25 },
      { date: '2011-10-19T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2011-06-15T00:00:00.000Z', grade: 'A', score: 10 }
    ],
    name: "Tony'S Deli",
    restaurant_id: '40363333',
    gradeCount: 6
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
