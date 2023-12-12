### Query

1.  db.restaurants.find( { "borough": { $nin: ["Staten Island", "Queens", "Bronx", "Brooklyn"] } }, { "restaurant_id": 1, "name": 1,
    "borough": 1, "cuisine": 1 });

- Expected Output -

```
[
  {
    _id: ObjectId("64758d35308eef6bfe3c4ed3"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: '1 East 66Th Street Kitchen',
    restaurant_id: '40359480'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ed5"),
    borough: 'Manhattan',
    cuisine: 'Irish',
    name: 'Dj Reynolds Pub And Restaurant',
    restaurant_id: '30191841'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ed9"),
    borough: 'Manhattan',
    cuisine: 'Delicatessen',
    name: "Bully'S Deli",
    restaurant_id: '40361708'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4edc"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Glorious Food',
    restaurant_id: '40361521'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4edd"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'P & S Deli Grocery',
    restaurant_id: '40362264'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ede"),
    borough: 'Manhattan',
    cuisine: 'Chicken',
    name: "Harriet'S Kitchen",
    restaurant_id: '40362098'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4edf"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Angelika Film Center',
    restaurant_id: '40362274'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee1"),
    borough: 'Manhattan',
    cuisine: 'Turkish',
    name: 'The Country Cafe',
    restaurant_id: '40362715'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee8"),
    borough: 'Manhattan',
    cuisine: 'Bakery',
    name: "Olive'S",
    restaurant_id: '40363151'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ee9"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Downtown Deli',
    restaurant_id: '40363021'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4eeb"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Cafe Metro',
    restaurant_id: '40363298'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4eed"),
    borough: 'Manhattan',
    cuisine: 'Sandwiches/Salads/Mixed Buffet',
    name: 'Lexler Deli',
    restaurant_id: '40363426'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef1"),
    borough: 'Manhattan',
    cuisine: 'Pizza',
    name: "Domino'S Pizza",
    restaurant_id: '40363644'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef2"),
    borough: 'Manhattan',
    cuisine: 'Pizza',
    name: "Domino'S Pizza",
    restaurant_id: '40363945'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef4"),
    borough: 'Manhattan',
    cuisine: 'Continental',
    name: "Lorenzo & Maria'S",
    restaurant_id: '40363630'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4ef5"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Spoon Bread Catering',
    restaurant_id: '40364179'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4efc"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Berkely',
    restaurant_id: '40363685'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4eff"),
    borough: 'Manhattan',
    cuisine: 'Chicken',
    name: 'Texas Rotisserie',
    restaurant_id: '40364304'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f00"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Palm Restaurant',
    restaurant_id: '40364355'
  },
  {
    _id: ObjectId("64758d35308eef6bfe3c4f01"),
    borough: 'Manhattan',
    cuisine: 'Italian',
    name: 'Isle Of Capri Resturant',
    restaurant_id: '40364373'
  }
]
```
