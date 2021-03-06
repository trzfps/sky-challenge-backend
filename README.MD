# *SKY - NODEJS CHALLENGE*

## **Dependencies**:
---

1. Docker
2. Docker Compose

## **Summary**:
---

1. Clone this repo;
2. Copy .env-example and create .env file 
2. Open your terminal;
3. Type the command `docker-compose up`;
4. Wait for nodemon to load and show two messages `Server is listing on port #`.
5. Done.


## **Endpoints**:
Below are listed all the endpoints in this microservice:

| Endpoint | Description | Need auth? |
|----------|-------------|------------|
| /signup | Register User  | no
| /signin | Sign in with User | no
| /user | Get user by Id | yes

## **Response types**:

*For development purposes*

---
### Success:


| Status |
|--------|
| 200    |

### Errors:

| Status | Type | Description |
|--------|------|-------------|
|  400   | Bad Request | Invalid data being submitted to any endpoint |
|  401   | Unauthorized | Request endpoints without providing access token |

### Response delivery (for Front-end purposes):
All the responses listed above are delivered in a JSON format. See example below:

```javascript
// Example with using user endpoint 
{
  "user": {
    "phones": [],
    "_id": "5db46d6abc3df603471d45b5",
    "name": "vitor",
    "email": "vitor_48@hotmail.com",
    "createdAt": "2019-10-26T15:59:38.831Z",
    "__v": 0,
    "lastLogin": "2019-10-26T16:47:45.884Z"
  }
}
