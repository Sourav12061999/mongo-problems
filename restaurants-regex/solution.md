### Query

1. db.restaurants.find({ name: { $regex: /pizza/i } }, { name: 1, address: 1 })

- Expected Output -

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d9495bc"),
    address: {
      building: '464',
      coord: [ -73.9791458, 40.744328 ],
      street: '3 Avenue',
      zipcode: '10016'
    },
    name: "Domino'S Pizza"
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495bd"),
    address: {
      building: '148',
      coord: [ -73.9806854, 40.7778589 ],
      street: 'West   72 Street',
      zipcode: '10023'
    },
    name: "Domino'S Pizza"
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495e9"),
    address: {
      building: '30-13',
      coord: [ -73.9151096, 40.763377 ],
      street: 'Steinway Street',
      zipcode: '11103'
    },
    name: "Rizzo'S Fine Pizza"
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495ec"),
    address: {
      building: '4035',
      coord: [ -73.9395182, 40.8422945 ],
      street: 'Broadway',
      zipcode: '10032'
    },
    name: 'Como Pizza'
  }
]
```
