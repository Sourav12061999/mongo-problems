<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find all restaurants with a grade of `A` and a score greater than `8`.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    _id: ObjectId("64758d35308eef6bfe3c4eda"),
    address: {
      building: '129-08',
      coord: [ -73.839297, 40.78147 ],
      street: '20 Avenue',
      zipcode: '11356'
    },
    borough: 'Queens',
    cuisine: 'Delicatessen',
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
    address: {
      building: '3406',
      coord: [ -73.94024739999999, 40.7623288 ],
      street: '10 Street',
      zipcode: '11106'
    },
    borough: 'Queens',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-03-19T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-03-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-03-27T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2011-04-05T00:00:00.000Z', grade: 'A', score: 7 }
    ],
    name: "Steve Chu'S Deli & Grocery",
    restaurant_id: '40361998'
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
