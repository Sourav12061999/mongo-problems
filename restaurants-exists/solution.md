### Query

1. db.restaurants.find( { "address.street": { $exists: true } });


- Expected Output -

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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-06-10T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2013-06-05T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-04-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-10-12T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-05-29T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2014-01-14T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-08-03T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-07-18T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-03-09T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-10-14T00:00:00.000Z', grade: 'A', score: 9 }
    ],
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
    borough: 'Staten Island',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-10-06T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2014-05-20T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-04-04T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-01-24T00:00:00.000Z', grade: 'A', score: 9 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Hamburgers',
    grades: [
      { date: '2014-12-30T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2014-07-01T00:00:00.000Z', grade: 'B', score: 23 },
      { date: '2013-04-30T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-05-08T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Bronx',
    cuisine: 'Bakery',
    grades: [
      { date: '2014-03-03T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-09-11T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2013-01-24T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2011-11-23T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-03-10T00:00:00.000Z', grade: 'B', score: 14 }
    ],
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
    borough: 'Queens',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-11-24T00:00:00.000Z', grade: 'Z', score: 20 },
      { date: '2013-01-17T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-08-02T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-12-15T00:00:00.000Z', grade: 'B', score: 25 }
    ],
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
    borough: 'Queens',
    cuisine: 'American',
    grades: [
      { date: '2014-11-15T00:00:00.000Z', grade: 'Z', score: 38 },
      { date: '2014-05-02T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-03-02T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-02-10T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-07-18T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-07-30T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-02-13T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-08-16T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2011-08-17T00:00:00.000Z', grade: 'A', score: 11 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-07-14T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-07-10T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-07-11T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2012-02-23T00:00:00.000Z', grade: 'A', score: 8 }
    ],
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
    borough: 'Bronx',
    cuisine: 'American',
    grades: [
      { date: '2014-05-28T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-06-19T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-06-15T00:00:00.000Z', grade: 'A', score: 3 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-04-16T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2013-04-23T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2012-04-24T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2011-12-16T00:00:00.000Z', grade: 'A', score: 2 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-11-10T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-10-10T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-10-04T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-05-21T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-12-30T00:00:00.000Z', grade: 'B', score: 19 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Chinese',
    grades: [
      { date: '2014-09-16T00:00:00.000Z', grade: 'B', score: 21 },
      { date: '2013-08-28T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2013-04-02T00:00:00.000Z', grade: 'C', score: 56 },
      { date: '2012-08-15T00:00:00.000Z', grade: 'B', score: 27 },
      { date: '2012-03-28T00:00:00.000Z', grade: 'B', score: 27 }
    ],
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
    borough: 'Manhattan',
    cuisine: 'American',
    grades: [
      { date: '2014-05-07T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-05-03T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-04-30T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2011-12-27T00:00:00.000Z', grade: 'A', score: 0 }
    ],
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
    borough: 'Queens',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-10-28T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-09-18T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-09-20T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Manhattan',
    cuisine: 'Irish',
    grades: [
      { date: '2014-09-06T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-07-22T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-07-31T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-12-29T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-02-10T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-01-02T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-01-09T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2011-11-07T00:00:00.000Z', grade: 'P', score: 12 },
      { date: '2011-07-21T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-08-21T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2014-03-05T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-01-10T00:00:00.000Z', grade: 'A', score: 10 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-11-19T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-11-14T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2012-12-05T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-05-17T00:00:00.000Z', grade: 'A', score: 11 }
    ],
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
  }
]
Type "it" for more
rest> db.restaurants.find( { "address.street": { $exists: true } });
[
  {
    _id: ObjectId("6447c9678dfeb17a7d949591"),
    address: {
      building: '2780',
      coord: [ -73.98241999999999, 40.579505 ],
      street: 'Stillwell Avenue',
      zipcode: '11224'
    },
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-06-10T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2013-06-05T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-04-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-10-12T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-05-29T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2014-01-14T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-08-03T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-07-18T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-03-09T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-10-14T00:00:00.000Z', grade: 'A', score: 9 }
    ],
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
    borough: 'Staten Island',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-10-06T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2014-05-20T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-04-04T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-01-24T00:00:00.000Z', grade: 'A', score: 9 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Hamburgers',
    grades: [
      { date: '2014-12-30T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2014-07-01T00:00:00.000Z', grade: 'B', score: 23 },
      { date: '2013-04-30T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-05-08T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Bronx',
    cuisine: 'Bakery',
    grades: [
      { date: '2014-03-03T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-09-11T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2013-01-24T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2011-11-23T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-03-10T00:00:00.000Z', grade: 'B', score: 14 }
    ],
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
    borough: 'Queens',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-11-24T00:00:00.000Z', grade: 'Z', score: 20 },
      { date: '2013-01-17T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-08-02T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-12-15T00:00:00.000Z', grade: 'B', score: 25 }
    ],
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
    borough: 'Queens',
    cuisine: 'American',
    grades: [
      { date: '2014-11-15T00:00:00.000Z', grade: 'Z', score: 38 },
      { date: '2014-05-02T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-03-02T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-02-10T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-07-18T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-07-30T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-02-13T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-08-16T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2011-08-17T00:00:00.000Z', grade: 'A', score: 11 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-07-14T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-07-10T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-07-11T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2012-02-23T00:00:00.000Z', grade: 'A', score: 8 }
    ],
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
    borough: 'Bronx',
    cuisine: 'American',
    grades: [
      { date: '2014-05-28T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-06-19T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-06-15T00:00:00.000Z', grade: 'A', score: 3 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-04-16T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2013-04-23T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2012-04-24T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2011-12-16T00:00:00.000Z', grade: 'A', score: 2 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-11-10T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-10-10T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-10-04T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-05-21T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-12-30T00:00:00.000Z', grade: 'B', score: 19 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Chinese',
    grades: [
      { date: '2014-09-16T00:00:00.000Z', grade: 'B', score: 21 },
      { date: '2013-08-28T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2013-04-02T00:00:00.000Z', grade: 'C', score: 56 },
      { date: '2012-08-15T00:00:00.000Z', grade: 'B', score: 27 },
      { date: '2012-03-28T00:00:00.000Z', grade: 'B', score: 27 }
    ],
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
    borough: 'Manhattan',
    cuisine: 'American',
    grades: [
      { date: '2014-05-07T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-05-03T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-04-30T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2011-12-27T00:00:00.000Z', grade: 'A', score: 0 }
    ],
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
    borough: 'Queens',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-10-28T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-09-18T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-09-20T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Manhattan',
    cuisine: 'Irish',
    grades: [
      { date: '2014-09-06T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-07-22T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-07-31T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-12-29T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-02-10T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-01-02T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-01-09T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2011-11-07T00:00:00.000Z', grade: 'P', score: 12 },
      { date: '2011-07-21T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-08-21T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2014-03-05T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-01-10T00:00:00.000Z', grade: 'A', score: 10 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-11-19T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-11-14T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2012-12-05T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-05-17T00:00:00.000Z', grade: 'A', score: 11 }
    ],
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
  }
]
Type "it" for more
rest> db.restaurants.find( { "address.street": { $exists: true } });
[
  {
    _id: ObjectId("6447c9678dfeb17a7d949591"),
    address: {
      building: '2780',
      coord: [ -73.98241999999999, 40.579505 ],
      street: 'Stillwell Avenue',
      zipcode: '11224'
    },
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-06-10T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2013-06-05T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-04-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-10-12T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-05-29T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2014-01-14T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-08-03T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-07-18T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-03-09T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-10-14T00:00:00.000Z', grade: 'A', score: 9 }
    ],
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
    borough: 'Staten Island',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-10-06T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2014-05-20T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-04-04T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-01-24T00:00:00.000Z', grade: 'A', score: 9 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Hamburgers',
    grades: [
      { date: '2014-12-30T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2014-07-01T00:00:00.000Z', grade: 'B', score: 23 },
      { date: '2013-04-30T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2012-05-08T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Bronx',
    cuisine: 'Bakery',
    grades: [
      { date: '2014-03-03T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-09-11T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2013-01-24T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2011-11-23T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-03-10T00:00:00.000Z', grade: 'B', score: 14 }
    ],
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
    borough: 'Queens',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-11-24T00:00:00.000Z', grade: 'Z', score: 20 },
      { date: '2013-01-17T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-08-02T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2011-12-15T00:00:00.000Z', grade: 'B', score: 25 }
    ],
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
    borough: 'Queens',
    cuisine: 'American',
    grades: [
      { date: '2014-11-15T00:00:00.000Z', grade: 'Z', score: 38 },
      { date: '2014-05-02T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-03-02T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-02-10T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-07-18T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-07-30T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-02-13T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-08-16T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2011-08-17T00:00:00.000Z', grade: 'A', score: 11 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-07-14T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-07-10T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-07-11T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2012-02-23T00:00:00.000Z', grade: 'A', score: 8 }
    ],
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
    borough: 'Bronx',
    cuisine: 'American',
    grades: [
      { date: '2014-05-28T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-06-19T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-06-15T00:00:00.000Z', grade: 'A', score: 3 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-04-16T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2013-04-23T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2012-04-24T00:00:00.000Z', grade: 'A', score: 5 },
      { date: '2011-12-16T00:00:00.000Z', grade: 'A', score: 2 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Jewish/Kosher',
    grades: [
      { date: '2014-11-10T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-10-10T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-10-04T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-05-21T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2011-12-30T00:00:00.000Z', grade: 'B', score: 19 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Chinese',
    grades: [
      { date: '2014-09-16T00:00:00.000Z', grade: 'B', score: 21 },
      { date: '2013-08-28T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2013-04-02T00:00:00.000Z', grade: 'C', score: 56 },
      { date: '2012-08-15T00:00:00.000Z', grade: 'B', score: 27 },
      { date: '2012-03-28T00:00:00.000Z', grade: 'B', score: 27 }
    ],
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
    borough: 'Manhattan',
    cuisine: 'American',
    grades: [
      { date: '2014-05-07T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-05-03T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-04-30T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2011-12-27T00:00:00.000Z', grade: 'A', score: 0 }
    ],
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
    borough: 'Queens',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-10-28T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2013-09-18T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-09-20T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Manhattan',
    cuisine: 'Irish',
    grades: [
      { date: '2014-09-06T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-07-22T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2012-07-31T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-12-29T00:00:00.000Z', grade: 'A', score: 12 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Ice Cream, Gelato, Yogurt, Ices',
    grades: [
      { date: '2014-02-10T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-01-02T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-01-09T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2011-11-07T00:00:00.000Z', grade: 'P', score: 12 },
      { date: '2011-07-21T00:00:00.000Z', grade: 'A', score: 13 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    grades: [
      { date: '2014-08-21T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2014-03-05T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-01-10T00:00:00.000Z', grade: 'A', score: 10 }
    ],
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
    borough: 'Brooklyn',
    cuisine: 'American',
    grades: [
      { date: '2014-11-19T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-11-14T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2012-12-05T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2012-05-17T00:00:00.000Z', grade: 'A', score: 11 }
    ],
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
  }
]
```
