### Queries

1. db.movies.find({ title: { $regex: /beginning/i } })


- Expected Output -

```
[
  {
    _id: ObjectId("64534bba33a02cd8aca2a309"),
    title: 'Baahubali: The Beginning',
    year: 2015,
    genre: [ 'Action', 'Drama' ],
    director: 'S. S. Rajamouli',
    cast: [ 'Prabhas', 'Rana Daggubati', 'Anushka Shetty' ],
    rating: 8.1,
    synopsis: 'In the kingdom of Mahishmati, Shivudu falls in love with a fair maiden named Avanthika, who is a member of a rebel group. When she asks him to help her in their fight against the tyrannical ruler, he agrees and finds out some shocking truths about his past.',
    runtime: 159,
    country: 'India'
  }
]
```
