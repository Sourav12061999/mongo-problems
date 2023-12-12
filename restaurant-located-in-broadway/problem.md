<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find the restaurants that are located on `Broadway` street and sort them by `zipcode` in `ascending` order.
- Limit the number of results to `10`.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    _id: ObjectId("64758d35308eef6bfe3c4ed9"),
    address: {
      building: '759',
      coord: [ -73.9925306, 40.7309346 ],
      street: 'Broadway',
      zipcode: '10003'
    },
    borough: 'Manhattan',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-01-21T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-01-04T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-06-07T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2012-01-17T00:00:00.000Z', grade: 'A', score: 8 }
    ],
    name: "Bully'S Deli",
    restaurant_id: '40361708'
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
    _id: ObjectId("64758d35308eef6bfe3c4f02"),
    address: {
      building: '178',
      coord: [ -73.96252129999999, 40.7098035 ],
      street: 'Broadway',
      zipcode: '11211'
    },
    borough: 'Brooklyn',
    cuisine: 'Steak',
    grades: [
      { date: '2014-03-08T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-09-28T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-03-26T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2012-09-10T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-08-15T00:00:00.000Z', grade: 'A', score: 13 }
    ],
    name: 'Peter Luger Steakhouse',
    restaurant_id: '40364335'
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
