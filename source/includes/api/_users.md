# Users

## Registration

To reginster as an user:

```shell
curl -X POST http://localhost:3000/register \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "user": {
      "email": "xyz@email.com",
      "nickname": "Username",
      "password": "password",
      "password_confirmation": "password",
      "name": "Anna Guay",
      "country_id": 2,
      "permissions_request": "ngo",
      "institution": "My organization"
  }
}'

## Log in

To login as an user:

```shell
curl -X POST http://localhost:3000/login \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "auth": {
      "email": "xyz@email.com",
      "password": "password"
  }
}'
```

<aside class="success">
Remember — the response is jsonapi format
</aside>

## Get current user

To obtain current user:

```shell
curl -X GET http://localhost:3000/users/current-user \
-H "Authorization: Bearer <your-token>" \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>

## How obtain all users

To obtain all users:

```shell
curl -X GET http://localhost:3000/users \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>

> Example response:

```json
{
  "data": [
    {
      "id": "1",
      "type": "users",
      "attributes": {
        "name": "Admin",
        "email": "admin@example.com",
        "country_id": 43,
        "nickname": "admin",
        "institution": null,
        "is_active": true,
        "deactivated_at": null
      },
      "relationships": {
        "user_permission": {
          "data": {
            "id": "1",
            "type": "user_permissions"
          }
        }
      }
    },
    {
      "id": "2",
      "type": "users",
      "attributes": {
        "name": "Web",
        "email": "webuser@example.com",
        "country_id": 43,
        "nickname": "webuser",
        "institution": null,
        "is_active": true,
        "deactivated_at": null
      },
      "relationships": {
        "user_permission": {
          "data": {
            "id": "2",
            "type": "user_permissions"
          }
        }
      }
    }
  ],
  "links": {
    "first": "http://localhost:3000/users?page%5Bnumber%5D=1",
    "prev": "http://localhost:3000/users?page%5Bnumber%5D=1",
    "next": "http://localhost:3000/users?page%5Bnumber%5D=1",
    "last": "http://localhost:3000/users?page%5Bnumber%5D=1"
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the users of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/users?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (name, created_at, updated_at) | Text


> To obtain all users sorted by name:

```shell
curl -X GET http://localhost:3000/users?sort=name \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/users?sort=-name \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific user

To obtain specific user:

```shell
curl -X GET http://localhost:3000/users/1 \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>

> Example response:

```json
{
  "data": {
    "id": "2",
    "type": "users",
    "attributes": {
      "name": "Web",
      "email": "webuser@example.com",
      "country_id": 43,
      "nickname": "webuser",
      "institution": null,
      "is_active": true,
      "deactivated_at": null
    },
    "relationships": {
      "user_permission": {
        "data": {
          "id": "2",
          "type": "user_permissions"
        }
      }
    }
  },
  "included": [
    {
      "id": "2",
      "type": "user_permissions",
      "attributes": {
        "user_id": 2,
        "user_role": "user",
        "permissions": {
          "user": {
            "id": [
              "manage"
            ]
          },
          "observation": {
            "all": [
              "read"
            ]
          }
        }
      }
    }
  ],
  "meta": {
    "updated_at": "2017-04-07T10:14:56.413Z",
    "created_at": "2017-04-07T10:14:56.413Z"
  }
}
```

## Creating an User

In order to create a user, you need an authorization token for current admin.

Only admin users should be able to create Users

To create a user, you need to define all of the required fields in the request body. The fields that compose a user are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| name                | Name of the user                                              | Text   | Any Text                                        | Yes
| email               | Email of the user                                             | Text   | Any valid email                                 | Yes
| password            | Password of the user                                          | Text   | Any valid password                              | Yes
| password_confirmation | Password confirmation of the user password                  | Text   | Any valid password                              | Yes
| nickname            | Username                                                      | Text   | Any Text                                        | Yes
| user_permission_attributes | User permissions (only accessible by admin)            | Hash   | {"user_role": "ngo" or "operator" or "admin"}                  | No
| institution         | User institution/company                                      | Text   | AnyText                                         | No
| is_active           | Activate deactiveta users (only accessible by admin and publisher) | Boolean  | default value false                      | No
| permissions_request | Permission request for user                                   | Text   | ngo, operator                                   | No


> To create an user, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/users \
-H "Authorization: Bearer <your-token>" \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "user": {
      "email": "xyz@email.com",
      "nickname": "Username",
      "password": "password",
      "password_confirmation": "password",
      "name": "Anna Guay",
      "country_id": 2,
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create user is an authenticated endpoint!
</aside>


## Updating an User

In order to modify the user, you can PUT/PATCH a request.
It accepts the same parameters as the _create user_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/users/<user-id> \
-H "Authorization: Bearer <your-token>" \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "user": {
      "name": "Another name for the user",
      "is_active": true
  }
}'
```

<aside class="notice">
Remember — create user is an authenticated endpoint!
</aside>

## Deleting an User
You can delete a user! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/users/<user-id> \
-H "Authorization: Bearer <your-token>" \
-H "SC_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create user is an authenticated endpoint!
</aside>
