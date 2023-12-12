<h1 style="color:#397ce7">Problem Description:</h1>

<h2 style="color:#397ce7">Problem Statement:</h2>

- Find all users email with _id who have a specific interest with `technology`?

<h4 style="color:#397ce7">Sample Output:</h4>

```json
[
  {
    "_id": 3,
    "email": "alice.johnson@example.com"
  },
  {
    "_id": 8,
    "email": "james.johnson@example.com"
  }
]
```

<h4 style="color:#397ce7">Sample Database:</h4>

```json
{
  "users": [
    {
      "_id": 1,
      "name": "John Doe",
      "email": "john.doe@example.com",
      "age": 30,
      "location": "New York",
      "interests": ["sports", "music", "travel"],
      "followers": [2, 3, 4, 5, 6, 7, 8, 9, 10],
      "following": [2, 3, 4, 5, 6, 7, 8, 9, 10]
    },
    {
      "_id": 2,
      "name": "Jane Smith",
      "email": "jane.smith@example.com",
      "age": 28,
      "location": "London",
      "interests": ["photography", "food", "books"],
      "followers": [1, 3, 4, 5, 6, 7, 8, 9, 10],
      "following": [1, 3, 4, 5, 6, 7, 8, 9, 10]
    },
    {
      "_id": 3,
      "name": "Alice Johnson",
      "email": "alice.johnson@example.com",
      "age": 32,
      "location": "San Francisco",
      "interests": ["technology", "art", "hiking"],
      "followers": [1, 2, 4, 5, 6, 7, 8, 9, 10],
      "following": [1, 2, 4, 5, 6, 7, 8, 9, 10]
    },
    {
      "_id": 4,
      "name": "Michael Brown",
      "email": "michael.brown@example.com",
      "age": 35,
      "location": "Chicago",
      "interests": ["movies", "cooking", "gaming"],
      "followers": [1, 2, 3, 5, 6, 7, 8, 9, 10],
      "following": [1, 2, 3, 5, 6, 7, 8, 9, 10]
    },
    {
      "_id": 5,
      "name": "Emma Wilson",
      "email": "emma.wilson@example.com",
      "age": 26,
      "location": "Sydney",
      "interests": ["fashion", "fitness", "beauty"],
      "followers": [1, 2, 3, 4, 6, 7, 8, 9, 10],
      "following": [1, 2, 3, 4, 6, 7, 8, 9, 10]
    },
    {
      "_id": 6,
      "name": "Daniel Miller",
      "email": "daniel.miller@example.com",
      "age": 29,
      "location": "Berlin",
      "interests": ["history", "nature", "languages"],
      "followers": [1, 2, 3, 4, 5, 7, 8, 9, 10],
      "following": [1, 2, 3, 4, 5, 7, 8, 9, 10]
    },
    {
      "_id": 7,
      "name": "Olivia Davis",
      "email": "olivia.davis@example.com",
      "age": 31,
      "location": "Paris",
      "interests": ["art", "travel", "music"],
      "followers": [1, 2, 3, 4, 5, 6, 8, 9, 10],
      "following": [1, 2, 3, 4, 5, 6, 8, 9, 10]
    },
    {
      "_id": 8,
      "name": "James Johnson",
      "email": "james.johnson@example.com",
      "age": 33,
      "location": "Toronto",
      "interests": ["technology", "coding", "gaming"],
      "followers": [1, 2, 3, 4, 5, 6, 7, 9, 10],
      "following": [1, 2, 3, 4, 5, 6, 7, 9, 10]
    },
    {
      "_id": 9,
      "name": "Sophia Thomas",
      "email": "sophia.thomas@example.com",
      "age": 27,
      "location": "Los Angeles",
      "interests": ["music", "movies", "travel"],
      "followers": [1, 2, 3, 4, 5, 6, 7, 8, 10],
      "following": [1, 2, 3, 4, 5, 6, 7, 8, 10]
    },
    {
      "_id": 10,
      "name": "Benjamin Clark",
      "email": "benjamin.clark@example.com",
      "age": 34,
      "location": "Melbourne",
      "interests": ["sports", "nature", "photography"],
      "followers": [1, 2, 3, 4, 5, 6, 7, 8, 9],
      "following": [1, 2, 3, 4, 5, 6, 7, 8, 9]
    }
  ],
  "posts": [
    {
      "_id": 1,
      "userId": 1,
      "content": "Hello, world!",
      "likes": [2, 3, 5, 6],
      "createdAt": "2023-05-30T10:00:00Z"
    },
    {
      "_id": 2,
      "userId": 2,
      "content": "This is amazing!",
      "likes": [1, 3, 4, 7],
      "createdAt": "2023-05-30T12:30:00Z"
    },
    {
      "_id": 3,
      "userId": 3,
      "content": "Check out this photo!",
      "likes": [2, 4, 5, 8],
      "createdAt": "2023-05-31T09:15:00Z"
    },
    {
      "_id": 4,
      "userId": 4,
      "content": "Having a great time!",
      "likes": [1, 5, 6, 7],
      "createdAt": "2023-05-31T11:45:00Z"
    },
    {
      "_id": 5,
      "userId": 5,
      "content": "New outfit!",
      "likes": [2, 3, 6, 8],
      "createdAt": "2023-06-01T14:20:00Z"
    },
    {
      "_id": 6,
      "userId": 6,
      "content": "Exploring new trails.",
      "likes": [1, 4, 7, 9],
      "createdAt": "2023-06-02T16:35:00Z"
    },
    {
      "_id": 7,
      "userId": 7,
      "content": "Enjoying the city lights.",
      "likes": [3, 5, 8, 9],
      "createdAt": "2023-06-03T19:10:00Z"
    },
    {
      "_id": 8,
      "userId": 8,
      "content": "Working on a new project.",
      "likes": [2, 4, 6, 10],
      "createdAt": "2023-06-04T21:55:00Z"
    },
    {
      "_id": 9,
      "userId": 9,
      "content": "Jamming with friends.",
      "likes": [1, 3, 7, 10],
      "createdAt": "2023-06-05T08:45:00Z"
    },
    {
      "_id": 10,
      "userId": 10,
      "content": "Nature's beauty!",
      "likes": [2, 5, 8, 9],
      "createdAt": "2023-06-06T12:20:00Z"
    },
    {
      "_id": 11,
      "userId": 1,
      "content": "Feeling motivated!",
      "likes": [3, 6, 9, 10],
      "createdAt": "2023-06-07T15:55:00Z"
    },
    {
      "_id": 12,
      "userId": 2,
      "content": "Trying new recipes.",
      "likes": [1, 4, 7, 8],
      "createdAt": "2023-06-08T18:30:00Z"
    },
    {
      "_id": 13,
      "userId": 3,
      "content": "Attending a tech conference.",
      "likes": [2, 5, 9, 10],
      "createdAt": "2023-06-09T22:05:00Z"
    },
    {
      "_id": 14,
      "userId": 4,
      "content": "Movie night with friends!",
      "likes": [1, 3, 6, 8],
      "createdAt": "2023-06-10T09:45:00Z"
    },
    {
      "_id": 15,
      "userId": 5,
      "content": "Beach day!",
      "likes": [2, 4, 7, 10],
      "createdAt": "2023-06-11T14:20:00Z"
    },
    {
      "_id": 16,
      "userId": 6,
      "content": "Learning a new language.",
      "likes": [1, 5, 8, 9],
      "createdAt": "2023-06-12T16:55:00Z"
    },
    {
      "_id": 17,
      "userId": 7,
      "content": "Art exhibition!",
      "likes": [3, 6, 9, 10],
      "createdAt": "2023-06-13T19:30:00Z"
    },
    {
      "_id": 18,
      "userId": 8,
      "content": "Game night with friends.",
      "likes": [2, 4, 7, 10],
      "createdAt": "2023-06-14T22:05:00Z"
    },
    {
      "_id": 19,
      "userId": 9,
      "content": "Road trip!",
      "likes": [1, 3, 6, 8],
      "createdAt": "2023-06-15T09:40:00Z"
    },
    {
      "_id": 20,
      "userId": 10,
      "content": "Sunset view.",
      "likes": [2, 5, 9, 10],
      "createdAt": "2023-06-16T12:15:00Z"
    },
    {
      "_id": 21,
      "userId": 1,
      "content": "Celebrating a milestone!",
      "likes": [3, 6, 9, 10],
      "createdAt": "2023-06-17T15:50:00Z"
    },
    {
      "_id": 22,
      "userId": 2,
      "content": "Weekend getaway.",
      "likes": [1, 4, 7, 8],
      "createdAt": "2023-06-18T18:25:00Z"
    },
    {
      "_id": 23,
      "userId": 3,
      "content": "Attending a music festival.",
      "likes": [2, 5, 9, 10],
      "createdAt": "2023-06-19T21:00:00Z"
    },
    {
      "_id": 24,
      "userId": 4,
      "content": "Trying out a new workout.",
      "likes": [1, 3, 6, 8],
      "createdAt": "2023-06-20T09:35:00Z"
    },
    {
      "_id": 25,
      "userId": 5,
      "content": "Exploring street food.",
      "likes": [2, 4, 7, 10],
      "createdAt": "2023-06-21T14:10:00Z"
    },
    {
      "_id": 26,
      "userId": 6,
      "content": "Relaxing in nature.",
      "likes": [1, 5, 8, 9],
      "createdAt": "2023-06-22T16:45:00Z"
    },
    {
      "_id": 27,
      "userId": 7,
      "content": "Live music concert.",
      "likes": [3, 6, 9, 10],
      "createdAt": "2023-06-23T19:20:00Z"
    },
    {
      "_id": 28,
      "userId": 8,
      "content": "Tech meetup.",
      "likes": [2, 4, 7, 10],
      "createdAt": "2023-06-24T21:55:00Z"
    },
    {
      "_id": 29,
      "userId": 9,
      "content": "Beach volleyball!",
      "likes": [1, 3, 6, 8],
      "createdAt": "2023-06-25T08:30:00Z"
    },
    {
      "_id": 30,
      "userId": 10,
      "content": "Sightseeing in the city.",
      "likes": [2, 5, 9, 10],
      "createdAt": "2023-06-26T12:05:00Z"
    }
  ],
  "comments": [
    {
      "_id": 1,
      "postId": 1,
      "userId": 2,
      "content": "Nice post!",
      "createdAt": "2023-05-30T11:00:00Z"
    },
    {
      "_id": 2,
      "postId": 1,
      "userId": 3,
      "content": "I agree!",
      "createdAt": "2023-05-30T11:15:00Z"
    },
    {
      "_id": 3,
      "postId": 2,
      "userId": 1,
      "content": "Absolutely!",
      "createdAt": "2023-05-30T13:00:00Z"
    },
    {
      "_id": 4,
      "postId": 3,
      "userId": 4,
      "content": "Beautiful photo!",
      "createdAt": "2023-05-31T09:30:00Z"
    },
    {
      "_id": 5,
      "postId": 3,
      "userId": 5,
      "content": "Where was this taken?",
      "createdAt": "2023-05-31T09:45:00Z"
    },
    {
      "_id": 6,
      "postId": 4,
      "userId": 6,
      "content": "Glad you're having a great time!",
      "createdAt": "2023-05-31T12:00:00Z"
    },
    {
      "_id": 7,
      "postId": 4,
      "userId": 7,
      "content": "Enjoy every moment!",
      "createdAt": "2023-05-31T12:30:00Z"
    },
    {
      "_id": 8,
      "postId": 5,
      "userId": 2,
      "content": "Love the outfit!",
      "createdAt": "2023-06-01T14:30:00Z"
    },
    {
      "_id": 9,
      "postId": 5,
      "userId": 3,
      "content": "You look amazing!",
      "createdAt": "2023-06-01T14:45:00Z"
    },
    {
      "_id": 10,
      "postId": 6,
      "userId": 4,
      "content": "Which trail is this?",
      "createdAt": "2023-06-02T16:45:00Z"
    },
    {
      "_id": 11,
      "postId": 6,
      "userId": 5,
      "content": "Looks so peaceful!",
      "createdAt": "2023-06-02T17:00:00Z"
    },
    {
      "_id": 12,
      "postId": 7,
      "userId": 6,
      "content": "City lights are mesmerizing!",
      "createdAt": "2023-06-03T19:30:00Z"
    },
    {
      "_id": 13,
      "postId": 7,
      "userId": 7,
      "content": "I love Paris!",
      "createdAt": "2023-06-03T19:45:00Z"
    },
    {
      "_id": 14,
      "postId": 8,
      "userId": 8,
      "content": "Can't wait to see the project!",
      "createdAt": "2023-06-04T22:00:00Z"
    },
    {
      "_id": 15,
      "postId": 8,
      "userId": 9,
      "content": "Keep up the good work!",
      "createdAt": "2023-06-04T22:15:00Z"
    },
    {
      "_id": 16,
      "postId": 9,
      "userId": 1,
      "content": "Wish I could join the jam session!",
      "createdAt": "2023-06-05T09:00:00Z"
    },
    {
      "_id": 17,
      "postId": 9,
      "userId": 2,
      "content": "Have fun!",
      "createdAt": "2023-06-05T09:15:00Z"
    },
    {
      "_id": 18,
      "postId": 10,
      "userId": 3,
      "content": "Nature's beauty is unparalleled!",
      "createdAt": "2023-06-06T12:30:00Z"
    },
    {
      "_id": 19,
      "postId": 10,
      "userId": 4,
      "content": "Gorgeous photo!",
      "createdAt": "2023-06-06T12:45:00Z"
    },
    {
      "_id": 20,
      "postId": 11,
      "userId": 5,
      "content": "You got this!",
      "createdAt": "2023-06-07T16:00:00Z"
    }
  ]
}
```
