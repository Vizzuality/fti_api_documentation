# Categories

## What is a Category?

A category is a group of categories for specific bussiness area.

## How to obtain all categories

> To obtain all categories:

```shell
curl -X GET http://localhost:3000/categories \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format and only accesible by admin or publisher user
</aside>

> Example response:

```json
{
  "data": [
    {
      "id": "3",
      "type": "categories",
      "attributes": {
        "name": "Payments"
      },
      "relationships": {
        "annex_governances": {
          "data": [
            {
              "id": "13",
              "type": "annex_governances"
            },
            {
              "id": "12",
              "type": "annex_governances"
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": "13",
              "type": "annex_operators"
            },
            {
              "id": "12",
              "type": "annex_operators"
            },
            {
              "id": "28",
              "type": "annex_operators"
            }
          ]
        }
      }
    },
    {
      "id": "4",
      "type": "categories",
      "attributes": {
        "name": "Right to exploit"
      },
      "relationships": {
        "annex_governances": {
          "data": []
        },
        "annex_operators": {
          "data": [
            {
              "id": "20",
              "type": "annex_operators"
            },
            {
              "id": "35",
              "type": "annex_operators"
            },
            {
              "id": "34",
              "type": "annex_operators"
            },
            {
              "id": "22",
              "type": "annex_operators"
            },
            {
              "id": "21",
              "type": "annex_operators"
            }
          ]
        }
      }
    },
    {
      "id": "1",
      "type": "categories",
      "attributes": {
        "name": "Social aspects"
      },
      "relationships": {
        "annex_governances": {
          "data": [
            {
              "id": "3",
              "type": "annex_governances"
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": "16",
              "type": "annex_operators"
            },
            {
              "id": "3",
              "type": "annex_operators"
            },
            {
              "id": "40",
              "type": "annex_operators"
            }
          ]
        }
      }
    },
    {
      "id": "6",
      "type": "categories",
      "attributes": {
        "name": "Timber harvesting"
      },
      "relationships": {
        "annex_governances": {
          "data": [
            {
              "id": "1",
              "type": "annex_governances"
            },
            {
              "id": "2",
              "type": "annex_governances"
            },
            {
              "id": "4",
              "type": "annex_governances"
            },
            {
              "id": "5",
              "type": "annex_governances"
            },
            {
              "id": "6",
              "type": "annex_governances"
            },
            {
              "id": "7",
              "type": "annex_governances"
            },
            {
              "id": "8",
              "type": "annex_governances"
            },
            {
              "id": "10",
              "type": "annex_governances"
            },
            {
              "id": "11",
              "type": "annex_governances"
            },
            {
              "id": "14",
              "type": "annex_governances"
            },
            {
              "id": "15",
              "type": "annex_governances"
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": "42",
              "type": "annex_operators"
            },
            {
              "id": "31",
              "type": "annex_operators"
            },
            {
              "id": "32",
              "type": "annex_operators"
            },
            {
              "id": "36",
              "type": "annex_operators"
            },
            {
              "id": "41",
              "type": "annex_operators"
            },
            {
              "id": "1",
              "type": "annex_operators"
            },
            {
              "id": "2",
              "type": "annex_operators"
            },
            {
              "id": "4",
              "type": "annex_operators"
            },
            {
              "id": "5",
              "type": "annex_operators"
            },
            {
              "id": "6",
              "type": "annex_operators"
            },
            {
              "id": "7",
              "type": "annex_operators"
            },
            {
              "id": "8",
              "type": "annex_operators"
            },
            {
              "id": "10",
              "type": "annex_operators"
            },
            {
              "id": "11",
              "type": "annex_operators"
            },
            {
              "id": "14",
              "type": "annex_operators"
            },
            {
              "id": "15",
              "type": "annex_operators"
            },
            {
              "id": "17",
              "type": "annex_operators"
            },
            {
              "id": "18",
              "type": "annex_operators"
            },
            {
              "id": "19",
              "type": "annex_operators"
            },
            {
              "id": "25",
              "type": "annex_operators"
            },
            {
              "id": "26",
              "type": "annex_operators"
            },
            {
              "id": "30",
              "type": "annex_operators"
            }
          ]
        }
      }
    },
    {
      "id": "2",
      "type": "categories",
      "attributes": {
        "name": "Timber processing"
      },
      "relationships": {
        "annex_governances": {
          "data": [
            {
              "id": "9",
              "type": "annex_governances"
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": "37",
              "type": "annex_operators"
            },
            {
              "id": "9",
              "type": "annex_operators"
            },
            {
              "id": "39",
              "type": "annex_operators"
            },
            {
              "id": "38",
              "type": "annex_operators"
            }
          ]
        }
      }
    },
    {
      "id": "5",
      "type": "categories",
      "attributes": {
        "name": "Timber transport / trade"
      },
      "relationships": {
        "annex_governances": {
          "data": []
        },
        "annex_operators": {
          "data": [
            {
              "id": "23",
              "type": "annex_operators"
            },
            {
              "id": "24",
              "type": "annex_operators"
            },
            {
              "id": "27",
              "type": "annex_operators"
            },
            {
              "id": "29",
              "type": "annex_operators"
            },
            {
              "id": "33",
              "type": "annex_operators"
            }
          ]
        }
      }
    }
  ],
  "links": {
    "first": "http://otp-staging.ipq.co/categories?page%5Bnumber%5D=1",
    "prev": "http://otp-staging.ipq.co/categories?page%5Bnumber%5D=1",
    "next": "http://otp-staging.ipq.co/categories?page%5Bnumber%5D=1",
    "last": "http://otp-staging.ipq.co/categories?page%5Bnumber%5D=1"
  },
  "meta": {
    "total_items": 6
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the categories of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/categories?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| type          | Filter by specific type (Solution, Bme, Impact, Enabling, Timing)        | Text
| sort          | Sort json response by specific attributes (name, created_at, updated_at) | Text


> To sort categories by name:

```shell
curl -X GET http://localhost:3000/categories?sort=name \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/categories?sort=-name \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain a specific category

> To obtain the category:

```shell
curl -X GET http://localhost:3000/categories/3 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```
> Example response:

```json
{
  "data": {
    "id": "3",
    "type": "categories",
    "attributes": {
      "name": "Payments"
    },
    "relationships": {
      "annex_governances": {
        "data": [
          {
            "id": 13,
            "created_at": "2017-04-06T16:24:46.300Z",
            "updated_at": "2017-04-06T16:24:46.317Z",
            "governance_pillar": "Planning and decision making",
            "governance_problem": "Non respect of procedures authorising harvesting of forest resources",
            "details": null
          },
          {
            "id": 12,
            "created_at": "2017-04-06T16:24:46.262Z",
            "updated_at": "2017-04-06T16:24:46.277Z",
            "governance_pillar": "Planning and decision making",
            "governance_problem": "Non respect of procedures - attribution of right to exploit, trade or transport CITES species",
            "details": null
          }
        ]
      },
      "annex_operators": {
        "data": [
          {
            "id": 28,
            "country_id": 228,
            "created_at": "2017-04-06T16:24:45.047Z",
            "updated_at": "2017-04-06T16:24:46.885Z",
            "illegality": "Export duty unpaid",
            "details": null
          },
          {
            "id": 12,
            "country_id": 53,
            "created_at": "2017-04-06T16:24:44.281Z",
            "updated_at": "2017-04-06T16:24:44.299Z",
            "illegality": "Default on fine payments",
            "details": null
          },
          {
            "id": 13,
            "country_id": 13,
            "created_at": "2017-04-06T16:24:44.332Z",
            "updated_at": "2017-04-06T16:25:18.168Z",
            "illegality": "Default on tax payments",
            "details": null
          }
        ]
      }
    }
  },
  "meta": {
    "updated_at": "2017-04-06T16:24:33.544Z",
    "created_at": "2017-04-06T16:24:33.544Z"
  }
}
```

<aside class="success">
Remember — the response is jsonapi format and only accessible by admin or publisher user
</aside>


## Creating a Category

In order to create a category, you need an authorization token for current user.

Only admin users should be able to create Categories

To create a category, you need to define all of the required fields in the request body. The fields that compose a category are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| name                | Name of the category                                    | Text   | Any Text                                        | Yes

> To create a category, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/categories \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
 '{
   "category": {
      "name":"Test category"
   }
}'
```
<aside class="notice">
  Remember that create category is an authenticated endpoint!
</aside>


## Updating a Category

In order to modify the category, you can PUT/PATCH a request.
It accepts the same parameters as the _create category_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/categories/<category-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "category": {
      "name": "Another name for the category"
  }
}'
```

<aside class="notice">
Remember — create category is an authenticated endpoint!
</aside>

## Deleting a Category
You can delete a category! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/categories/<category-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create category is an authenticated endpoint!
</aside>
