### Query

1. db.restaurants.find( { "address.coord.1": { $gt: 10, $lte: 41 } }, { "restaurant_id": 1, "name": 1, "address": 1, "coord": 1 });

- Expected Output

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d949591"),
    address: {
      building: '2780',
      coord: [ -73.98241999999999, 40.579505 ],
      street: 'Stillwell Avenue',
      zipcode: '11224'
    },
    name: 'Riviera Caterer',
    restaurant_id: '40356018'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949592"),
    address: {
      building: '7114',
      coord: [ -73.9068506, 40.6199034 ],
      street: 'Avenue U',
      zipcode: '11234'
    },
    name: "Wilken'S Fine Food",
    restaurant_id: '40356483'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949593"),
    address: {
      building: '2206',
      coord: [ -74.1377286, 40.6119572 ],
      street: 'Victory Boulevard',
      zipcode: '10314'
    },
    name: 'Kosher Island',
    restaurant_id: '40356442'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949594"),
    address: {
      building: '469',
      coord: [ -73.961704, 40.662942 ],
      street: 'Flatbush Avenue',
      zipcode: '11225'
    },
    name: "Wendy'S",
    restaurant_id: '30112340'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949595"),
    address: {
      building: '1007',
      coord: [ -73.856077, 40.848447 ],
      street: 'Morris Park Ave',
      zipcode: '10462'
    },
    name: 'Morris Park Bake Shop',
    restaurant_id: '30075445'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949596"),
    address: {
      building: '97-22',
      coord: [ -73.8601152, 40.7311739 ],
      street: '63 Road',
      zipcode: '11374'
    },
    name: 'Tov Kosher Kitchen',
    restaurant_id: '40356068'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949597"),
    address: {
      building: '8825',
      coord: [ -73.8803827, 40.7643124 ],
      street: 'Astoria Boulevard',
      zipcode: '11369'
    },
    name: 'Brunos On The Boulevard',
    restaurant_id: '40356151'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949598"),
    address: {
      building: '6409',
      coord: [ -74.00528899999999, 40.628886 ],
      street: '11 Avenue',
      zipcode: '11219'
    },
    name: 'Regina Caterers',
    restaurant_id: '40356649'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d949599"),
    address: {
      building: '1839',
      coord: [ -73.9482609, 40.6408271 ],
      street: 'Nostrand Avenue',
      zipcode: '11226'
    },
    name: 'Taste The Tropics Ice Cream',
    restaurant_id: '40356731'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959a"),
    address: {
      building: '2300',
      coord: [ -73.8786113, 40.8502883 ],
      street: 'Southern Boulevard',
      zipcode: '10460'
    },
    name: 'Wild Asia',
    restaurant_id: '40357217'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959b"),
    address: {
      building: '7715',
      coord: [ -73.9973325, 40.61174889999999 ],
      street: '18 Avenue',
      zipcode: '11214'
    },
    name: 'C & C Catering Service',
    restaurant_id: '40357437'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959c"),
    address: {
      building: '705',
      coord: [ -73.9653967, 40.6064339 ],
      street: 'Kings Highway',
      zipcode: '11223'
    },
    name: 'Seuda Foods',
    restaurant_id: '40360045'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959d"),
    address: {
      building: '1269',
      coord: [ -73.871194, 40.6730975 ],
      street: 'Sutter Avenue',
      zipcode: '11208'
    },
    name: 'May May Kitchen',
    restaurant_id: '40358429'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959e"),
    address: {
      building: '1',
      coord: [ -73.96926909999999, 40.7685235 ],
      street: 'East   66 Street',
      zipcode: '10065'
    },
    name: '1 East 66Th Street Kitchen',
    restaurant_id: '40359480'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959f"),
    address: {
      building: '265-15',
      coord: [ -73.7032601, 40.7386417 ],
      street: 'Hillside Avenue',
      zipcode: '11004'
    },
    name: 'Carvel Ice Cream',
    restaurant_id: '40361322'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a0"),
    address: {
      building: '351',
      coord: [ -73.98513559999999, 40.7676919 ],
      street: 'West   57 Street',
      zipcode: '10019'
    },
    name: 'Dj Reynolds Pub And Restaurant',
    restaurant_id: '30191841'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a1"),
    address: {
      building: '203',
      coord: [ -73.97822040000001, 40.6435254 ],
      street: 'Church Avenue',
      zipcode: '11218'
    },
    name: 'Carvel Ice Cream',
    restaurant_id: '40360076'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a2"),
    address: {
      building: '6909',
      coord: [ -74.0259567, 40.6353674 ],
      street: '3 Avenue',
      zipcode: '11209'
    },
    name: 'Nordic Delicacies',
    restaurant_id: '40361390'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a3"),
    address: {
      building: '284',
      coord: [ -73.9829239, 40.6580753 ],
      street: 'Prospect Park West',
      zipcode: '11215'
    },
    name: 'The Movable Feast',
    restaurant_id: '40361606'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a4"),
    address: {
      building: '759',
      coord: [ -73.9925306, 40.7309346 ],
      street: 'Broadway',
      zipcode: '10003'
    },
    name: "Bully'S Deli",
    restaurant_id: '40361708'
  }
]
```
