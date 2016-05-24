# json-mock-server

在后台services不能连通的情况下，实现完全脱离后台的前端mock数据。

$ json-server

$ npm install json-mock-kuitos -g

$ npm install -g json-server



---creat db.json

    {
      "users": [
        { "id": 1, "name": "kuitos", "location": "China"},
        { "id": 2, "name": "visiting-user", "location": "UK"}
      ],
      "posts": [
        { "id": 1, "title": "json-mock", "body":"The internet is cool!", "author": "therebelrobot", "userId": 1 }
      ],
      "comments": [
        { "id": 1, "body": "some comment from author", "votes": 20, "postId": 1, "userId": 1 },
        { "id": 2, "body": "some comment from visitor", "votes": 15, "postId": 1, "userId": 2 }
      ]
    }
    
---creat json server

    $ npm install -g json-server
      
---Start JSON Server

    $ json-server --watch db.json
