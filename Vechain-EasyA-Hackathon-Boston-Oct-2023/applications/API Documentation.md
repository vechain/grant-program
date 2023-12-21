# Sozo inFashion API Reference

## Description 
Sozo's REST API is structured in a way that allows developers to easily fetch data, make user-specific updates, and understand the information being provided. All responses are in JSON format and use standard HTTP response codes.

| Base URL    | 
| ----------- | 
| `https://sozo.api.com`   |

## Endpoints
### Users
**GET** /user/list

Returns a list of all users.
| Parameter     | Type        | Description 
| -----------   | ----------- | ----------- |  
| limit          | `integer`    | `optional` Maximum number of users to return; Default is 20.  |

**Reponse**

Returns an array objects containing the following data.
| Key           | Type        | Description 
| -----------   | ----------- | ----------- |
| id            | `integer`   | Auto-incremented value assigned when user is created in the database |
| username      | `string`    | The name a user's enters for login; Also the name displayed to other users in the app. |
| role          | `string`    | A user's role (either "designer" or "client") |

**Example**

Request:
```
GET /users/list?limit=42
```
Response:
```json
[
  {
  "id": 1,
  "username": "DrewDream",
  "role": "designer"
  },
  {
  "id": 2,
  "username": "TaylorJ",
  "role": "client"
  },
  // ...
]
```

`POST`

`DELETE`
***
### Clients
***
### Designers
***
### Sessions
