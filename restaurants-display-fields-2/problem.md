<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Write a MongoDB query to display the fields `restaurant_id`, `name`, `borough` and `cuisine`, but `exclude` the field `_id` for all the documents in the collection restaurant.

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "borough": "Brooklyn",
    "cuisine": "American",
    "name": "Riviera Caterer",
    "restaurant_id": "40356018"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "Delicatessen",
    "name": "Wilken'S Fine Food",
    "restaurant_id": "40356483"
  },
  {
    "borough": "Staten Island",
    "cuisine": "Jewish/Kosher",
    "name": "Kosher Island",
    "restaurant_id": "40356442"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "Hamburgers",
    "name": "Wendy'S",
    "restaurant_id": "30112340"
  },
  {
    "borough": "Bronx",
    "cuisine": "Bakery",
    "name": "Morris Park Bake Shop",
    "restaurant_id": "30075445"
  },
  {
    "borough": "Queens",
    "cuisine": "Jewish/Kosher",
    "name": "Tov Kosher Kitchen",
    "restaurant_id": "40356068"
  },
  {
    "borough": "Queens",
    "cuisine": "American",
    "name": "Brunos On The Boulevard",
    "restaurant_id": "40356151"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "American",
    "name": "Regina Caterers",
    "restaurant_id": "40356649"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "Ice Cream, Gelato, Yogurt, Ices",
    "name": "Taste The Tropics Ice Cream",
    "restaurant_id": "40356731"
  },
  {
    "borough": "Bronx",
    "cuisine": "American",
    "name": "Wild Asia",
    "restaurant_id": "40357217"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "American",
    "name": "C & C Catering Service",
    "restaurant_id": "40357437"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "Jewish/Kosher",
    "name": "Seuda Foods",
    "restaurant_id": "40360045"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "Chinese",
    "name": "May May Kitchen",
    "restaurant_id": "40358429"
  },
  {
    "borough": "Manhattan",
    "cuisine": "American",
    "name": "1 East 66Th Street Kitchen",
    "restaurant_id": "40359480"
  },
  {
    "borough": "Queens",
    "cuisine": "Ice Cream, Gelato, Yogurt, Ices",
    "name": "Carvel Ice Cream",
    "restaurant_id": "40361322"
  },
  {
    "borough": "Manhattan",
    "cuisine": "Irish",
    "name": "Dj Reynolds Pub And Restaurant",
    "restaurant_id": "30191841"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "Ice Cream, Gelato, Yogurt, Ices",
    "name": "Carvel Ice Cream",
    "restaurant_id": "40360076"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "Delicatessen",
    "name": "Nordic Delicacies",
    "restaurant_id": "40361390"
  },
  {
    "borough": "Brooklyn",
    "cuisine": "American",
    "name": "The Movable Feast",
    "restaurant_id": "40361606"
  },
  {
    "borough": "Manhattan",
    "cuisine": "Delicatessen",
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
