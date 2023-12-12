### Problem Description

## Given below movies json data to perform mongo queries.

```
 [
  {
    "title": "Baahubali: The Beginning",
    "year": 2015,
    "genre": ["Action", "Drama"],
    "director": "S. S. Rajamouli",
    "cast": [
      "Prabhas",
      "Rana Daggubati",
      "Anushka Shetty"
    ],
    "rating": 8.1,
    "synopsis": "In the kingdom of Mahishmati, Shivudu falls in love with a fair maiden named Avanthika, who is a member of a rebel group. When she asks him to help her in their fight against the tyrannical ruler, he agrees and finds out some shocking truths about his past.",
    "runtime": 159,
    "country": "India"
  },
  {
    "title": "Dangal",
    "year": 2016,
    "genre": ["Biography", "Drama", "Sport"],
    "director": "Nitesh Tiwari",
    "cast": [
      "Aamir Khan",
      "Sakshi Tanwar",
      "Fatima Sana Shaikh"
    ],
    "rating": 8.4,
    "synopsis": "The story of a former wrestler and his two wrestler daughters who struggle towards glory at the Commonwealth Games in the face of societal oppression.",
    "runtime": 161,
    "country": "India"
  },
  {
    "title": "Lagaan",
    "year": 2001,
    "genre": ["Drama", "Musical", "Sport"],
    "director": "Ashutosh Gowariker",
    "cast": [
      "Aamir Khan",
      "Gracy Singh",
      "Rachel Shelley"
    ],
    "rating": 8.1,
    "synopsis": "In 1890s India, an arrogant British commander challenges the harshly taxed residents of a poor village to a cricket match, in an attempt to salvage his reputation and career.",
    "runtime": 224,
    "country": "India"
  },
  {
    "title": "3 Idiots",
    "year": 2009,
    "genre": ["Comedy", "Drama"],
    "director": "Rajkumar Hirani",
    "cast": [
      "Aamir Khan",
      "Kareena Kapoor",
      "Madhavan"
    ],
    "rating": 8.4,
    "synopsis": "Two friends are searching for their long lost companion. They revisit their college days and recall the memories of their friend who inspired them to think differently, even as the rest of the world called them 'idiots'.",
    "runtime": 170,
    "country": "India"
  },
  {
    "title": "Gangs of Wasseypur",
    "year": 2012,
    "genre": ["Action", "Crime", "Drama"],
    "director": "Anurag Kashyap",
    "cast": [
      "Manoj Bajpayee",
      "Nawazuddin Siddiqui",
      "Richa Chadha"
    ],
    "rating": 8.2,
    "synopsis": "A clash between Sultan and Shahid Khan leads to the expulsion of Khan from Wasseypur, and ignites a deadly blood feud spanning three generations.",
    "runtime": 321,
    "country": "India"
  }]
```

- Problem - write query to Find the `average rating` of all movies ?
- hint - use aggregation to perform operations (group together with `_id = nll`)
