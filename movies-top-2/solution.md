### Queries

1. db.movies.aggregate([ { $sort: { rating: -1 } }, { $limit: 2 }]);

- Expected Output -

```
[
  {
    _id: ObjectId("64534bba33a02cd8aca2a30c"),
    title: '3 Idiots',
    year: 2009,
    genre: [ 'Comedy', 'Drama' ],
    director: 'Rajkumar Hirani',
    cast: [ 'Aamir Khan', 'Kareena Kapoor', 'Madhavan' ],
    rating: 8.4,
    synopsis: "Two friends are searching for their long lost companion. They revisit their college days and recall the memories of their friend who inspired them to think differently, even as the rest of the world called them 'idiots'.",
    runtime: 170,
    country: 'India'
  },
  {
    _id: ObjectId("64534bba33a02cd8aca2a30a"),
    title: 'Dangal',
    year: 2016,
    genre: [ 'Biography', 'Drama', 'Sport' ],
    director: 'Nitesh Tiwari',
    cast: [ 'Aamir Khan', 'Sakshi Tanwar', 'Fatima Sana Shaikh' ],
    rating: 8.4,
    synopsis: 'The story of a former wrestler and his two wrestler daughters who struggle towards glory at the Commonwealth Games in the face of societal oppression.',
    runtime: 161,
    country: 'India'
  }
]
```
