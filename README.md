# minarest API for Demo

## Get all posts

  GET http://mina.creg.vn/posts
  
### Response

```json

[
  {
    "_id": "590ca7518b9f2c78568ac06a",
    "title": "Bai viet 11242000",
    "link": "http://vnexpress.net",
    "content": "Communication",
    "__v": 0,
    "created_date": "2017-05-05T16:24:49.932Z"
  },
  {
    "_id": "590ca7748b9f2c78568ac06b",
    "title": "Vietnam que huong toi",
    "link": "http://vnexpress.net/vietnam.jpg",
    "content": "Sample content",
    "__v": 0,
    "created_date": "2017-05-05T16:25:24.287Z"
  },
  {
    "_id": "590ca77d8b9f2c78568ac06c",
    "title": "Vietnam que huong toi 2",
    "link": "http://vnexpress.net/vietnam2.jpg",
    "content": "Sample content",
    "__v": 0,
    "created_date": "2017-05-05T16:25:33.351Z"
  }
]

```

## Get post details

  GET http://mina.creg.vn/posts/:id (Example: http://mina.creg.vn/posts/590ca7518b9f2c78568ac06a)
  
### Response

```json
{
    "_id": "590ca7518b9f2c78568ac06a",
    "title": "Bai viet 11242000",
    "link": "http://vnexpress.net",
    "content": "Communication",
    "__v": 0,
    "created_date": "2017-05-05T16:24:49.932Z"
}
```

## Create new post 

### Request
  POST http://mina.creg.vn/posts
Header
```
Content-type: application/json
```
Body Example
```json
{
  "title": "Vietnam que huong toi 2",
  "link": "http://vnexpress.net/vietnam2.jpg",
  "content": "Sample content"
}

```
### Response
```json
{
    "_id": "590ca7518b9f2c78568ac06a",
    "title": "Bai viet 11242000",
    "link": "http://vnexpress.net",
    "content": "Communication",
    "__v": 0,
    "created_date": "2017-05-05T16:24:49.932Z"
}
```

## Update post by :id

### Request
  PATCH http://mina.creg.vn/posts/:id (Example:  http://mina.creg.vn/posts/590ca7518b9f2c78568ac06a)
Header
```
Content-type: application/json
```
Body Example
```json
{
  "title": "Vietnam que huong toi 2",
  "link": "http://vnexpress.net/vietnam2.jpg",
  "content": "Sample content"
}

```
### Response
```json
{
    "_id": "590ca7518b9f2c78568ac06a",
    "title": "Bai viet 11242000",
    "link": "http://vnexpress.net",
    "content": "Communication",
    "__v": 0,
    "created_date": "2017-05-05T16:24:49.932Z"
}
```

## Remove post by :id

### Request
  DELETE http://mina.creg.vn/posts/:id (Example:  http://mina.creg.vn/posts/590ca7518b9f2c78568ac06a)
### Response
```json
{
   "message":"Successful Deleted!!"
}
```



