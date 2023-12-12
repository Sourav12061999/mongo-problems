### Queries

1. db.movies.aggregate([
   { $group: { _id: "$year", count: { $sum: 1 } } }
   ]);

- Expected Output -

```
{ "_id": 2016, "count": 1 }
{ "_id": 2015, "count": 1 }
{ "_id": 2001, "count": 1 }
{ "_id": 2009, "count": 1 }
{ "_id": 2012, "count": 1 }

```
