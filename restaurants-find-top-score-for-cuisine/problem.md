<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find the top `5` restaurants with the highest `average score` for each cuisine type, along with their average scores.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "cuisine": "Steak",
    "topRestaurants": [
      { "restaurant_id": "40364335", "avgScore": 10 },
      { "restaurant_id": "40364572", "avgScore": 7.4 }
    ]
  },
  {
    "cuisine": "Chicken",
    "topRestaurants": [
      { "restaurant_id": "40364304", "avgScore": 17.6 },
      { "restaurant_id": "40362098", "avgScore": 10.666666666666666 }
    ]
  },
  {
    "cuisine": "Jewish/Kosher",
    "topRestaurants": [
      { "restaurant_id": "40356068", "avgScore": 17.75 },
      { "restaurant_id": "40364529", "avgScore": 12.333333333333334 },
      { "restaurant_id": "40360045", "avgScore": 11.8 },
      { "restaurant_id": "40356442", "avgScore": 10.5 },
      { "restaurant_id": "40364220", "avgScore": 10 }
    ]
  },
  {
    "cuisine": "Pizza",
    "topRestaurants": [
      { "restaurant_id": "40365280", "avgScore": 21.5 },
      { "restaurant_id": "40363945", "avgScore": 13.25 },
      { "restaurant_id": "40364920", "avgScore": 9.2 },
      { "restaurant_id": "40363644", "avgScore": 5.333333333333333 }
    ]
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
