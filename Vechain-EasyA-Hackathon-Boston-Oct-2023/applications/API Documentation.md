# Sozo inFashion API Reference

## Description 
Sozo's REST API is structured in a way that allows developers to easily fetch data, make user-specific updates, and understand the information being provided. All responses are in JSON format and use standard HTTP response codes.

| Base URL    | 
| ----------- | 
| `https://sozo.api.com`   |

## Endpoints
```http
GET /users
GET /users/{user_id}
POST /users/create
PATCH /users/{user_id}
DELETE /users/{user_id}

GET /requests/{request_id}
POST /requests
DELETE /requests/{request_id}

GET /pieces
GET /pieces/{piece_id}
POST /pieces/create
PATCH /pieces/{piece_id}
```

### Users
**GET** /users

Returns a list of all designer users.
| Parameter     | Type        | Description 
| -----------   | ----------- | ----------- |  
| limit          | `integer`    | `optional` Maximum number of designer users to return; Default is 20.  |
| role          | `string`    | `optional` Type of users to return ('designer' or 'client')  |

**Reponse**

Returns an array of objects containing the following data.
| Key           | Type        | Description 
| -----------   | ----------- | ----------- |
| designer_id   | `string`   | Unique value assigned when user is created in the database. |
| username      | `string`    | The name a user's enters for login; Also the name displayed to other users in the app. |
| role          | `string`    | A user's role (always "designer"). |
| first_name    | `string`    | A user's first name. |
| last_name     | `string`    | A user's last name. |
| active_status | `number`    | 1 to indicate active **OR** 0 to indicate not active |

**Example**

Request:
```
GET /designers?limit=42
```
Response:
```json
[
  {
  "designer_id": "hTwR4QEXHYPf7Ua6tjjM",
  "username": "DrewDream",
  "role": "designer",
  "first_name": "Drew",
  "last_name": "Thompson"
  },
  {
  "designer_id": "Hfkq7urNonHMonGREKU3",
  "username": "TaylorJ",
  "role": "designer",
  "first_name": "Taylor",
  "last_name": "Joslin"
  },
  {...}
]
```

**GET** /designers/:id

Returns an object representing a single designer user.
| Parameter     | 
| ----------- |  
| No parameters  |

**Reponse**

Returns a single user object containing the following data.
| Key           | Type        | Description 
| -----------   | ----------- | ----------- |
| designer_id   | `string`   | Unique value assigned when user is created in the database. |
| username      | `string`    | The name a user's enters for login; Also the name displayed to other users in the app. |
| role          | `string`    | A user's role (always "designer"). |
| first_name    | `string`    | A user's first name. |
| last_name     | `string`    | A user's last name. |
| active_status    | `binary`    | 1 to indicate active **OR** 0 to indicate not active |

**Example**

Request:
```
GET /users/4aMvjt3NnNTAeDdM5tri
```
Response:
```json
{
  "designer_id": "hTwR4QEXHYPf7Ua6tjjM",
  "username": "DrewDream",
  "role": "designer",
  "first_name": "Drew",
  "last_name": "Thompson"
}
```

`POST`

`DELETE`

Returns an object representing a single designer user.
| Parameter     | 
| ----------- |  
| No parameters  |

**Reponse**

Returns an object containing the following data:
| Key           | Type        | Description 
| -----------   | ----------- | ----------- |
| designer_id   | `string`   | Unique value assigned when user is created in the database. |
| username      | `string`    | The name a user's enters for login; Also the name displayed to other users in the app. |
| deleted | `boolean`    | `true` to indicate account was successfully deleted **OR** `false` to indicate the account was not deleted. |

**Example**

Request:
```
DELETE /users/4aMvjt3NnNTAeDdM5tri
```
Response:
```json
{
  "designer_id": "hTwR4QEXHYPf7Ua6tjjM",
  "username": "DrewDream",
  "deleted": true
}
```

***
### Clients
***
### Designers
***
### Sessions
