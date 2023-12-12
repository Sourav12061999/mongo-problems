### Query

1.  db.restaurants.find({},{"restaurant_id" : 1,"name":1,"borough":1,"address.zipcode" :1,"_id":0})

- Expected Output

```
[
  {
    address: { zipcode: '11224' },
    borough: 'Brooklyn',
    name: 'Riviera Caterer',
    restaurant_id: '40356018'
  },
  {
    address: { zipcode: '11234' },
    borough: 'Brooklyn',
    name: "Wilken'S Fine Food",
    restaurant_id: '40356483'
  },
  {
    address: { zipcode: '10314' },
    borough: 'Staten Island',
    name: 'Kosher Island',
    restaurant_id: '40356442'
  },
  {
    address: { zipcode: '11225' },
    borough: 'Brooklyn',
    name: "Wendy'S",
    restaurant_id: '30112340'
  },
  {
    address: { zipcode: '10462' },
    borough: 'Bronx',
    name: 'Morris Park Bake Shop',
    restaurant_id: '30075445'
  },
  {
    address: { zipcode: '11374' },
    borough: 'Queens',
    name: 'Tov Kosher Kitchen',
    restaurant_id: '40356068'
  },
  {
    address: { zipcode: '11369' },
    borough: 'Queens',
    name: 'Brunos On The Boulevard',
    restaurant_id: '40356151'
  },
  {
    address: { zipcode: '11219' },
    borough: 'Brooklyn',
    name: 'Regina Caterers',
    restaurant_id: '40356649'
  },
  {
    address: { zipcode: '11226' },
    borough: 'Brooklyn',
    name: 'Taste The Tropics Ice Cream',
    restaurant_id: '40356731'
  },
  {
    address: { zipcode: '10460' },
    borough: 'Bronx',
    name: 'Wild Asia',
    restaurant_id: '40357217'
  },
  {
    address: { zipcode: '11214' },
    borough: 'Brooklyn',
    name: 'C & C Catering Service',
    restaurant_id: '40357437'
  },
  {
    address: { zipcode: '11223' },
    borough: 'Brooklyn',
    name: 'Seuda Foods',
    restaurant_id: '40360045'
  },
  {
    address: { zipcode: '11208' },
    borough: 'Brooklyn',
    name: 'May May Kitchen',
    restaurant_id: '40358429'
  },
  {
    address: { zipcode: '10065' },
    borough: 'Manhattan',
    name: '1 East 66Th Street Kitchen',
    restaurant_id: '40359480'
  },
  {
    address: { zipcode: '11004' },
    borough: 'Queens',
    name: 'Carvel Ice Cream',
    restaurant_id: '40361322'
  },
  {
    address: { zipcode: '10019' },
    borough: 'Manhattan',
    name: 'Dj Reynolds Pub And Restaurant',
    restaurant_id: '30191841'
  },
  {
    address: { zipcode: '11218' },
    borough: 'Brooklyn',
    name: 'Carvel Ice Cream',
    restaurant_id: '40360076'
  },
  {
    address: { zipcode: '11209' },
    borough: 'Brooklyn',
    name: 'Nordic Delicacies',
    restaurant_id: '40361390'
  },
  {
    address: { zipcode: '11215' },
    borough: 'Brooklyn',
    name: 'The Movable Feast',
    restaurant_id: '40361606'
  },
  {
    address: { zipcode: '10003' },
    borough: 'Manhattan',
    name: "Bully'S Deli",
    restaurant_id: '40361708'
  }
]
```
