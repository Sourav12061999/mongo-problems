### Query

1.

```json
db.restaurants.find({ $and: [ { $or: [{ borough: "Manhattan" }, { borough: "Brooklyn" }] }, { "grades.score": { $lt: 5 } }, { cuisine: { $ne: "American" } }] })
```

- Expected Output

```
[
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
    _id: ObjectId("6447c9678dfeb17a7d9495ab"),
    address: {
      building: '531',
      coord: [ -73.9634876, 40.6940001 ],
      street: 'Myrtle Avenue',
      zipcode: '11205'
    },
    borough: 'Brooklyn',
    cuisine: 'Hamburgers',
    grades: [
      { date: '2014-03-18T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2013-03-18T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-10-10T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2011-09-22T00:00:00.000Z', grade: 'A', score: 2 }
    ],
    name: 'White Castle',
    restaurant_id: '40362344'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495ad"),
    address: {
      building: '195',
      coord: [ -73.9246028, 40.6522396 ],
      street: 'East   56 Street',
      zipcode: '11203'
    },
    borough: 'Brooklyn',
    cuisine: 'Caribbean',
    grades: [
      { date: '2014-05-13T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-05-08T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-09-22T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2011-06-06T00:00:00.000Z', grade: 'A', score: 12 }
    ],
    name: "Shashemene Int'L Restaura",
    restaurant_id: '40362869'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495b3"),
    address: {
      building: '120',
      coord: [ -73.9998042, 40.7251256 ],
      street: 'Prince Street',
      zipcode: '10012'
    },
    borough: 'Manhattan',
    cuisine: 'Bakery',
    grades: [
      { date: '2014-10-17T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-09-18T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2013-04-30T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-04-20T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2011-12-19T00:00:00.000Z', grade: 'A', score: 3 }
    ],
    name: "Olive'S",
    restaurant_id: '40363151'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495b8"),
    address: {
      building: '405',
      coord: [ -73.97534999999999, 40.7516269 ],
      street: 'Lexington Avenue',
      zipcode: '10174'
    },
    borough: 'Manhattan',
    cuisine: 'Sandwiches/Salads/Mixed Buffet',
    grades: [
      { date: '2014-02-21T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2013-09-13T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2012-08-28T00:00:00.000Z', grade: 'A', score: 0 },
      { date: '2011-09-13T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-05-03T00:00:00.000Z', grade: 'A', score: 5 }
    ],
    name: 'Lexler Deli',
    restaurant_id: '40363426'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495bc"),
    address: {
      building: '464',
      coord: [ -73.9791458, 40.744328 ],
      street: '3 Avenue',
      zipcode: '10016'
    },
    borough: 'Manhattan',
    cuisine: 'Pizza',
    grades: [
      { date: '2014-08-05T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2014-03-06T00:00:00.000Z', grade: 'A', score: 11 },
      { date: '2013-07-09T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-01-30T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2012-01-05T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2011-09-26T00:00:00.000Z', grade: 'A', score: 0 }
    ],
    name: "Domino'S Pizza",
    restaurant_id: '40363644'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495c6"),
    address: {
      building: '976',
      coord: [ -73.92701509999999, 40.6620192 ],
      street: 'Rutland Road',
      zipcode: '11212'
    },
    borough: 'Brooklyn',
    cuisine: 'Chinese',
    grades: [
      { date: '2014-04-23T00:00:00.000Z', grade: 'A', score: 13 },
      { date: '2013-03-26T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2012-03-13T00:00:00.000Z', grade: 'A', score: 4 },
      { date: '2011-11-16T00:00:00.000Z', grade: 'A', score: 13 }
    ],
    name: 'Golden Pavillion',
    restaurant_id: '40363920'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495cd"),
    address: {
      building: '178',
      coord: [ -73.96252129999999, 40.7098035 ],
      street: 'Broadway',
      zipcode: '11211'
    },
    borough: 'Brooklyn',
    cuisine: 'Steak',
    grades: [
      { date: '2014-03-08T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-09-28T00:00:00.000Z', grade: 'A', score: 10 },
      { date: '2013-03-26T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2012-09-10T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2011-08-15T00:00:00.000Z', grade: 'A', score: 13 }
    ],
    name: 'Peter Luger Steakhouse',
    restaurant_id: '40364335'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495d7"),
    address: {
      building: '845',
      coord: [ -73.965531, 40.765431 ],
      street: 'Lexington Avenue',
      zipcode: '10065'
    },
    borough: 'Manhattan',
    cuisine: 'Steak',
    grades: [
      { date: '2014-03-26T00:00:00.000Z', grade: 'A', score: 12 },
      { date: '2013-03-21T00:00:00.000Z', grade: 'A', score: 8 },
      { date: '2012-10-18T00:00:00.000Z', grade: 'A', score: 9 },
      { date: '2012-05-07T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2011-05-17T00:00:00.000Z', grade: 'A', score: 5 }
    ],
    name: "Donohue'S Steak House",
    restaurant_id: '40364572'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495dc"),
    address: {
      building: '261',
      coord: [ -73.94839189999999, 40.7224876 ],
      street: 'Driggs Avenue',
      zipcode: '11222'
    },
    borough: 'Brooklyn',
    cuisine: 'Polish',
    grades: [
      { date: '2014-05-31T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-05-10T00:00:00.000Z', grade: 'A', score: 3 },
      { date: '2012-02-17T00:00:00.000Z', grade: 'A', score: 6 },
      { date: '2011-10-14T00:00:00.000Z', grade: 'C', score: 54 }
    ],
    name: 'Polish National Home',
    restaurant_id: '40364404'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495f0"),
    address: {
      building: '1616',
      coord: [ -73.952449, 40.776325 ],
      street: '2 Avenue',
      zipcode: '10028'
    },
    borough: 'Manhattan',
    cuisine: 'Irish',
    grades: [
      { date: '2014-02-28T00:00:00.000Z', grade: 'A', score: 2 },
      { date: '2013-08-30T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2012-08-27T00:00:00.000Z', grade: 'A', score: 7 },
      { date: '2011-09-14T00:00:00.000Z', grade: 'A', score: 9 }
    ],
    name: "Dorrian'S Red Hand Restaurant",
    restaurant_id: '40365239'
  }
]
```
