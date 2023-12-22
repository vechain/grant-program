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
***
## Users

**GET** /users

Returns a list of all designer users.
| Parameter     | Type        | Description 
| -----------   | :-----------: | ----------- |  
| limit          | `integer`    | `optional` Maximum number of designer users to return; Default is 20.  |
| role          | `string`    | `optional` Type of users to return ('designer' or 'client')  |

**Response**

Returns an array of objects containing the following data.
| Key           | Type        | Description 
| -----------   | :-----------: | ----------- |
| user_id       | `string`    | Unique value assigned when user is created in the database. |
| username      | `string`    | A user's display name; Also used for login. |
| email         | `string`    | A user's email address. |
| role          | `string`    | A user's role ('designer' or 'client'). |
| first_name    | `string`    | A user's first name. |
| last_name     | `string`    | A user's last name. |
| bio           | `string`    | A description of the user. |
| active_status | `number`    | 1 indicates **active** **OR** 0 indicates **not active** |

**Example**

Request:
```http
GET /users?limit=2
```
Response:
```json
[
  {
    "user_id": "hTwR4QEXHYPf7Ua6tjjM",
    "username": "DrewDream",
    "email": "dreamlife@yahoo.com",
    "role": "designer",
    "first_name": "Drew",
    "last_name": "Thompson"
    "bio": "Bold stitches, fierce fabrics. Transforming threads into masterpieces. 🧵✨ #FashionAlchemy #StyleVisionary",
    "active_status": 1
  },
  {
    "user_id": "Hfkq7urNonHMonGREKU3",
    "username": "TaylorJ",
    "email": "taylor.joslin@gmail.com",
    "role": "client",
    "first_name": "Taylor",
    "last_name": "Joslin",
    "bio": "Dedicated to refining elegance through precision. Crafting timeless designs with meticulous attention to detail. Fashion designer focused on timeless style.",
    "active_status": 1
  }
]
```
***
**GET** /users/{user_id}

Retrieve a single user account.
| Parameter     | 
| ----------- |  
| No parameters  |

**Reponse**

Returns a single user object containing the following data.
| Key           | Type        | Description 
| -----------   | :-----------: | ----------- |
| user_id   | `string`   | Unique value assigned when user is created in the database. |
| username      | `string`    | A user's display name. |
| email      | `string`    | A user's email address. |
| role          | `string`    | A user's role ('designer' or 'client'). |
| first_name    | `string`    | A user's first name. |
| last_name     | `string`    | A user's last name. |
| bio     | `string`    | A description of the user (max length: 200 characters). |
| active_status | `number`    | 1 indicates **active** **OR** 0 indicates **not active** |

**Example**

Request:
```http
GET /users/hTwR4QEXHYPf7Ua6tjjM
```
Response:
```json
{
  "user_id": "hTwR4QEXHYPf7Ua6tjjM",
  "username": "DrewDream",
  "role": "designer",
  "first_name": "Drew",
  "last_name": "Thompson",
  "bio": "Bold stitches, fierce fabrics. Transforming threads into masterpieces. 🧵✨ #FashionAlchemy #StyleVisionary",
  "active_status": 1
}
```
***
**POST** /users/create

Creates a new user account.
| Parameter     | Type        | Description 
| -----------   | :-----------: | ----------- |  
| username      | `string`    | `required` A user's display name. Does not allow special chatacters; Can be used for login. |
| email         | `string`    | `required` A user's email address; Can be used for login. |
| role          | `string`    | `required` A user's role ('designer' or 'client'). |
| first_name    | `string`    | `required` A user's first name. |
| last_name     | `string`    | `required` A user's last name. |
| bio           | `string`    | `optional` A description of the user (max length: 200 characters). |

**Response**

Returns a single user object containing the following data.

| Key           | Type        | Description 
| -----------   | ----------- | ----------- |
| user_id       | `string`    | Unique value assigned when user is created in the database. |
| username      | `string`    | A user's display name. |
| email         | `string`    | A user's email address. |
| role          | `string`    | A user's role ('designer' or 'client'). |
| first_name    | `string`    | A user's first name. |
| last_name     | `string`    | A user's last name. |
| bio           | `string`    | A description of the user. |
| active_status | `number`    | 1 indicates **active** **OR** 0 indicates **not active** |

**Example**

Request:
```http
POST /users/create?username=RachelY&email=rachel.yearny%40gmail.com&role=client&first_name=Rachel&last_name=Yearny
```
Response:
```json
{
  "user_id": "H094iAjZyPWr4rm0y9WL",
  "username": "RachelY",
  "email": "rachel.yearny@gmail.com",
  "role": "client",
  "first_name": "Rachel",
  "last_name": "Yearny",
  "bio": "",
  "active_status": 1
}
```
***
**PATCH** /users/{user_id}

Update parts of a user's profile information.
| Parameter     | Type        | Description 
| -----------   | :-----------: | ----------- |  
| username      | `string`    | `optional` A user's display name. Does not allow special chatacters; Can be used for login. |
| email         | `string`    | `optional` A user's email address. |
| first_name    | `string`    | `optional` A user's first name. |
| last_name     | `string`    | `optional` A user's last name. |
| bio           | `string`    | `optional` A description of the user. |

**Response**

Returns a single user object containing the following data.

| Key           | Type        | Description 
| -----------   | ----------- | ----------- |
| user_id       | `string`    | Unique value assigned when user is created in the database. |
| username      | `string`    | A user's display name. |
| email         | `string`    | A user's email address. |
| role          | `string`    | A user's role ('designer' or 'client'). |
| first_name    | `string`    | A user's first name. |
| last_name     | `string`    | A user's last name. |
| bio           | `string`    | A description of the user. |
| active_status | `number`    | 1 indicates **active** **OR** 0 indicates **not active** |

**Example**

Request:
```http
PATCH /users/H094iAjZyPWr4rm0y9WL?username=YearOfRachel&bio="Sculpting%20sophistication%20in%20every%20stitch.%20Empowering%20women%20through%20distinctive%20designs.%20Committed%20to%20redefining%20style%20with%20grace%20and%20purpose."
```
Response:
```json
{
  "user_id": "H094iAjZyPWr4rm0y9WL",
  "username": "YearOfRachel",
  "email": "rachel.yearny@gmail.com",
  "role": "client",
  "first_name": "Rachel",
  "last_name": "Yearny",
  "bio": "Sculpting sophistication in every stitch. Empowering women through distinctive designs. Committed to redefining style with grace and purpose.",
  "active_status": 1
}
```
***
**DELETE** /users/{user_id}

Returns an object representing a single user.
| Parameter     | 
| ----------- |  
| No parameters  |

**Reponse**

Returns an object containing the following data:
| Key           | Type        | Description 
| -----------   | ----------- | ----------- |
| user_id   | `string`   | Unique value assigned when user is created in the database. |
| username      | `string`    | A user's display name. |
| deleted | `boolean`    | `true` to indicate account was successfully deleted **OR** `false` to indicate the account was not deleted. |

**Example**

Request:
```
DELETE /users/hTwR4QEXHYPf7Ua6tjjM
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
### Requests
***
### Pieces
***
