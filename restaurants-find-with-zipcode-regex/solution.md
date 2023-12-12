### Query

1.

```json
db.restaurants.aggregate([ { $unwind: "$address" }, { $match: { "address.zipcode": /^10/ } }, { $project: { "address.building":1, "address.coord":1,name: 1, "address.street": 1, "address.zipcode": 1, _id: 0 } }])
```

- Expected Output -

```
[
  {
    address: {
      building: '2206',
      coord: [ -74.1377286, 40.6119572 ],
      street: 'Victory Boulevard',
      zipcode: '10314'
    },
    name: 'Kosher Island'
  },
  {
    address: {
      building: '1007',
      coord: [ -73.856077, 40.848447 ],
      street: 'Morris Park Ave',
      zipcode: '10462'
    },
    name: 'Morris Park Bake Shop'
  },
  {
    address: {
      building: '2300',
      coord: [ -73.8786113, 40.8502883 ],
      street: 'Southern Boulevard',
      zipcode: '10460'
    },
    name: 'Wild Asia'
  },
  {
    address: {
      building: '1',
      coord: [ -73.96926909999999, 40.7685235 ],
      street: 'East   66 Street',
      zipcode: '10065'
    },
    name: '1 East 66Th Street Kitchen'
  },
  {
    address: {
      building: '351',
      coord: [ -73.98513559999999, 40.7676919 ],
      street: 'West   57 Street',
      zipcode: '10019'
    },
    name: 'Dj Reynolds Pub And Restaurant'
  },
  {
    address: {
      building: '759',
      coord: [ -73.9925306, 40.7309346 ],
      street: 'Broadway',
      zipcode: '10003'
    },
    name: "Bully'S Deli"
  },
  {
    address: {
      building: '522',
      coord: [ -73.95171, 40.767461 ],
      street: 'East   74 Street',
      zipcode: '10021'
    },
    name: 'Glorious Food'
  },
  {
    address: {
      building: '730',
      coord: [ -73.96805719999999, 40.7925587 ],
      street: 'Columbus Avenue',
      zipcode: '10025'
    },
    name: 'P & S Deli Grocery'
  },
  {
    address: {
      building: '502',
      coord: [ -73.976112, 40.786714 ],
      street: 'Amsterdam Avenue',
      zipcode: '10024'
    },
    name: "Harriet'S Kitchen"
  },
  {
    address: {
      building: '18',
      coord: [ -73.996984, 40.72589 ],
      street: 'West Houston Street',
      zipcode: '10012'
    },
    name: 'Angelika Film Center'
  },
  {
    address: {
      building: '60',
      coord: [ -74.0085357, 40.70620539999999 ],
      street: 'Wall Street',
      zipcode: '10005'
    },
    name: 'The Country Cafe'
  },
  {
    address: {
      building: '1006',
      coord: [ -73.84856870000002, 40.8903781 ],
      street: 'East 233 Street',
      zipcode: '10466'
    },
    name: 'Carvel Ice Cream'
  },
  {
    address: {
      building: '1236',
      coord: [ -73.8893654, 40.81376179999999 ],
      street: '238 Spofford Ave',
      zipcode: '10474'
    },
    name: 'Happy Garden'
  },
  {
    address: {
      building: '120',
      coord: [ -73.9998042, 40.7251256 ],
      street: 'Prince Street',
      zipcode: '10012'
    },
    name: "Olive'S"
  },
  {
    address: {
      building: '107',
      coord: [ -74.00920839999999, 40.7132925 ],
      street: 'Church Street',
      zipcode: '10007'
    },
    name: 'Downtown Deli'
  },
  {
    address: {
      building: '625',
      coord: [ -73.990494, 40.7569545 ],
      street: '8 Avenue',
      zipcode: '10018'
    },
    name: 'Cafe Metro'
  },
  {
    address: {
      building: '2491',
      coord: [ -74.1459332, 40.6103714 ],
      street: 'Victory Boulevard',
      zipcode: '10314'
    },
    name: 'Bagels N Buns'
  },
  {
    address: {
      building: '405',
      coord: [ -73.97534999999999, 40.7516269 ],
      street: 'Lexington Avenue',
      zipcode: '10174'
    },
    name: 'Lexler Deli'
  },
  {
    address: {
      building: '1111',
      coord: [ -74.0796436, 40.59878339999999 ],
      street: 'Hylan Boulevard',
      zipcode: '10305'
    },
    name: 'Carvel Ice Cream'
  },
  {
    address: {
      building: '464',
      coord: [ -73.9791458, 40.744328 ],
      street: '3 Avenue',
      zipcode: '10016'
    },
    name: "Domino'S Pizza"
  }
]
```
