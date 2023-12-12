<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to find the `average score` for each restaurant.
- <span style="color:red">Hint:</span> use aggregation to group all `_id=name` and use $unwind
- avgScore - name for key to store average score

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  { "_id": "Sonny'S Heros", "avgScore": 4.333333333333333 },
  { "_id": "Harriet'S Kitchen", "avgScore": 10.666666666666666 },
  { "_id": "Donohue'S Steak House", "avgScore": 7.4 },
  { "_id": "Melody Lanes", "avgScore": 12.25 },
  { "_id": "Shell Lanes", "avgScore": 15.6 },
  { "_id": "Polish National Home", "avgScore": 16.25 },
  { "_id": "Downtown Deli", "avgScore": 11 },
  { "_id": "La Grenouille", "avgScore": 10.666666666666666 },
  { "_id": "Texas Rotisserie", "avgScore": 17.6 },
  { "_id": "Seuda Foods", "avgScore": 11.8 },
  { "_id": "Great Kills Yacht Club", "avgScore": 7.333333333333333 },
  { "_id": "Mejlander & Mulgannon", "avgScore": 9.75 },
  { "_id": "White Castle", "avgScore": 6.25 },
  { "_id": "Kosher Island", "avgScore": 10.5 },
  { "_id": "The Country Cafe", "avgScore": 10.5 },
  { "_id": "Glorious Food", "avgScore": 12.2 },
  { "_id": "Hot Bagels", "avgScore": 19.166666666666668 },
  { "_id": "B & M Hot Bagel & Grocery", "avgScore": 15.6 },
  { "_id": "Marchis Restaurant", "avgScore": 19 },
  { "_id": "Golden Pavillion", "avgScore": 10 }
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
