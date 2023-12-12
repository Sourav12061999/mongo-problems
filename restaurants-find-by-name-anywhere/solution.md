### Query

1. db.restaurants.find( { "name": /.*Reg.*/ }, { "restaurant_id": 1, "name": 1, "borough": 1, "cuisine": 1 });

- Expected Output -

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d949598"),
    borough: 'Brooklyn',
    cuisine: 'American',
    name: 'Regina Caterers',
    restaurant_id: '40356649'
  }
]
```
