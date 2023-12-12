<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find the name and address of the restaurants that have a `zipcode` that starts with `10`.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "address": {
      "building": "2206",
      "coord": [-74.1377286, 40.6119572],
      "street": "Victory Boulevard",
      "zipcode": "10314"
    },
    "name": "Kosher Island"
  },
  {
    "address": {
      "building": "1007",
      "coord": [-73.856077, 40.848447],
      "street": "Morris Park Ave",
      "zipcode": "10462"
    },
    "name": "Morris Park Bake Shop"
  },
  {
    "address": {
      "building": "2300",
      "coord": [-73.8786113, 40.8502883],
      "street": "Southern Boulevard",
      "zipcode": "10460"
    },
    "name": "Wild Asia"
  },
  {
    "address": {
      "building": "1",
      "coord": [-73.96926909999999, 40.7685235],
      "street": "East   66 Street",
      "zipcode": "10065"
    },
    "name": "1 East 66Th Street Kitchen"
  },
  {
    "address": {
      "building": "351",
      "coord": [-73.98513559999999, 40.7676919],
      "street": "West   57 Street",
      "zipcode": "10019"
    },
    "name": "Dj Reynolds Pub And Restaurant"
  },
  {
    "address": {
      "building": "759",
      "coord": [-73.9925306, 40.7309346],
      "street": "Broadway",
      "zipcode": "10003"
    },
    "name": "Bully'S Deli"
  },
  {
    "address": {
      "building": "522",
      "coord": [-73.95171, 40.767461],
      "street": "East   74 Street",
      "zipcode": "10021"
    },
    "name": "Glorious Food"
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
