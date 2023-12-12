<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to display the fields `restaurant_id`, `name`, `borough` and `zip code`, but `exclude` the field `_id` for all the documents in the collection restaurant.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "address": { "zipcode": "11224" },
    "borough": "Brooklyn",
    "name": "Riviera Caterer",
    "restaurant_id": "40356018"
  },
  {
    "address": { "zipcode": "11234" },
    "borough": "Brooklyn",
    "name": "Wilken'S Fine Food",
    "restaurant_id": "40356483"
  },
  {
    "address": { "zipcode": "10314" },
    "borough": "Staten Island",
    "name": "Kosher Island",
    "restaurant_id": "40356442"
  },
  {
    "address": { "zipcode": "11225" },
    "borough": "Brooklyn",
    "name": "Wendy'S",
    "restaurant_id": "30112340"
  },
  {
    "address": { "zipcode": "10462" },
    "borough": "Bronx",
    "name": "Morris Park Bake Shop",
    "restaurant_id": "30075445"
  },
  {
    "address": { "zipcode": "11374" },
    "borough": "Queens",
    "name": "Tov Kosher Kitchen",
    "restaurant_id": "40356068"
  },
  {
    "address": { "zipcode": "11369" },
    "borough": "Queens",
    "name": "Brunos On The Boulevard",
    "restaurant_id": "40356151"
  },
  {
    "address": { "zipcode": "11219" },
    "borough": "Brooklyn",
    "name": "Regina Caterers",
    "restaurant_id": "40356649"
  },
  {
    "address": { "zipcode": "11226" },
    "borough": "Brooklyn",
    "name": "Taste The Tropics Ice Cream",
    "restaurant_id": "40356731"
  },
  {
    "address": { "zipcode": "10460" },
    "borough": "Bronx",
    "name": "Wild Asia",
    "restaurant_id": "40357217"
  },
  {
    "address": { "zipcode": "11214" },
    "borough": "Brooklyn",
    "name": "C & C Catering Service",
    "restaurant_id": "40357437"
  },
  {
    "address": { "zipcode": "11223" },
    "borough": "Brooklyn",
    "name": "Seuda Foods",
    "restaurant_id": "40360045"
  },
  {
    "address": { "zipcode": "11208" },
    "borough": "Brooklyn",
    "name": "May May Kitchen",
    "restaurant_id": "40358429"
  },
  {
    "address": { "zipcode": "10065" },
    "borough": "Manhattan",
    "name": "1 East 66Th Street Kitchen",
    "restaurant_id": "40359480"
  },
  {
    "address": { "zipcode": "11004" },
    "borough": "Queens",
    "name": "Carvel Ice Cream",
    "restaurant_id": "40361322"
  },
  {
    "address": { "zipcode": "10019" },
    "borough": "Manhattan",
    "name": "Dj Reynolds Pub And Restaurant",
    "restaurant_id": "30191841"
  },
  {
    "address": { "zipcode": "11218" },
    "borough": "Brooklyn",
    "name": "Carvel Ice Cream",
    "restaurant_id": "40360076"
  },
  {
    "address": { "zipcode": "11209" },
    "borough": "Brooklyn",
    "name": "Nordic Delicacies",
    "restaurant_id": "40361390"
  },
  {
    "address": { "zipcode": "11215" },
    "borough": "Brooklyn",
    "name": "The Movable Feast",
    "restaurant_id": "40361606"
  },
  {
    "address": { "zipcode": "10003" },
    "borough": "Manhattan",
    "name": "Bully'S Deli",
    "restaurant_id": "40361708"
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
