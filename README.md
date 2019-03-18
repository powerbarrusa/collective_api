
## Install

cd collective-api
npm install
npm start
```

Then you can see the API running on [http://localhost:8082](http://localhost:8082)

### Project: React Inbox
- GET (all messages): `http://localhost:8082/api/messages`
- PATCH (updates multiple messages, see API for req.body requirements): `http://localhost:8082/api/messages`  
``` Example req.body to mark messages 1,2,3 as read
{
  "messageIds": [1,2,3],
  "command": "read",
  "read": true
}
