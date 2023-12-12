### Queries

1. db.movies.find({ rating: { $gte: 8.2, $lte: 8.3 } })


- Expected Output -

```
[
  {
    _id: ObjectId("64534bba33a02cd8aca2a30d"),
    title: 'Gangs of Wasseypur',
    year: 2012,
    genre: [ 'Action', 'Crime', 'Drama' ],
    director: 'Anurag Kashyap',
    cast: [ 'Manoj Bajpayee', 'Nawazuddin Siddiqui', 'Richa Chadha' ],
    rating: 8.2,
    synopsis: 'A clash between Sultan and Shahid Khan leads to the expulsion of Khan from Wasseypur, and ignites a deadly blood feud spanning three generations.',
    runtime: 321,
    country: 'India'
  }
]
```
