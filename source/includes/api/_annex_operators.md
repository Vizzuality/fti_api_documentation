# AnnexOperators

## How obtain all annex_operators

To obtain all annex_operators:

```shell
curl -X GET http://localhost:3000/annex_operators \
-H "OTP-API-KEY: Bearer <your-api-key>" \
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
      "type": "annex_operators",
      "attributes": {
        "illegality": "Abandonment of timber ",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "13",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "1",
              "type": "severities"
            },
            {
              "id": "2",
              "type": "severities"
            },
            {
              "id": "3",
              "type": "severities"
            },
            {
              "id": "4",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "202",
              "type": "laws"
            },
            {
              "id": "203",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "2",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Timber laundering",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "13",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "5",
              "type": "severities"
            },
            {
              "id": "6",
              "type": "severities"
            },
            {
              "id": "7",
              "type": "severities"
            },
            {
              "id": "8",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": []
        }
      }
    },
    {
      "id": "34",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Company not registered according to regulations",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "13",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "133",
              "type": "severities"
            },
            {
              "id": "134",
              "type": "severities"
            },
            {
              "id": "135",
              "type": "severities"
            },
            {
              "id": "136",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "4",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": []
        }
      }
    },
    {
      "id": "3",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Insufficient consultation of local/indigenous populations ",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "194",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "9",
              "type": "severities"
            },
            {
              "id": "10",
              "type": "severities"
            },
            {
              "id": "11",
              "type": "severities"
            },
            {
              "id": "12",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "1",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "98",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "4",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Harvesting non authorised species",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "13",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "13",
              "type": "severities"
            },
            {
              "id": "14",
              "type": "severities"
            },
            {
              "id": "15",
              "type": "severities"
            },
            {
              "id": "16",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "189",
              "type": "laws"
            },
            {
              "id": "190",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "5",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Harvesting in a protected area or other area where logging is prohibited",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "234",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "17",
              "type": "severities"
            },
            {
              "id": "18",
              "type": "severities"
            },
            {
              "id": "19",
              "type": "severities"
            },
            {
              "id": "20",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": []
        }
      }
    },
    {
      "id": "6",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Cutting outside permit boundaries",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "13",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "21",
              "type": "severities"
            },
            {
              "id": "22",
              "type": "severities"
            },
            {
              "id": "23",
              "type": "severities"
            },
            {
              "id": "24",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "23",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "7",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Cutting trees below minimum diameter",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "13",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "25",
              "type": "severities"
            },
            {
              "id": "26",
              "type": "severities"
            },
            {
              "id": "27",
              "type": "severities"
            },
            {
              "id": "28",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": []
        }
      }
    },
    {
      "id": "8",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Cutting trees below minimum diameter",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "53",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "29",
              "type": "severities"
            },
            {
              "id": "30",
              "type": "severities"
            },
            {
              "id": "31",
              "type": "severities"
            },
            {
              "id": "32",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "5",
              "type": "laws"
            }
          ]
        }
      }
    }
  ],
  "links": {
    "first": "http://localhost:3000/annex_operators?page%5Bnumber%5D=1",
    "prev": "http://localhost:3000/annex_operators?page%5Bnumber%5D=1",
    "next": "http://localhost:3000/annex_operators?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://localhost:3000/annex_operators?page%5Bnumber%5D=5&page%5Bsize%5D=10",
    "self": "http://localhost:3000/annex_operators?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the annex_operators of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/annex_operators?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (illegality, created_at, updated_at) | Text


> To obtain all annex_operators sorted by illegality:

```shell
curl -X GET http://localhost:3000/annex_operators?sort=illegality \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/annex_operators?sort=-illegality \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific annex_operator

To obtain specific annex_operator:

```shell
curl -X GET http://localhost:3000/annex_operators/33 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a AnnexOperator

In order to create a annex_operator, you need an authorization token for current admin.

Only admin should be able to create AnnexOperators

To create a annex_operator, you need to define all of the required fields in the request body. The fields that compose a annex_operator are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| illegality          | Name of the illegality                                        | Text    | Any Text                                        | Yes
| country_id          | ID of country                                                 | Integer | Any Text                                        | No
| details             | Datails - description                                         | Text    | Any Text                                        | No

> To create a annex_operator, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/annex_operators \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "annex_operator": {
      "illegality": "Art. 100",
      "details": "Problem",
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create annex_operator is an authenticated endpoint!
</aside>


## Updating a AnnexOperator

In order to modify the annex_operator, you can PUT/PATCH a request.
It accepts the same parameters as the _create annex_operator_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/annex_operators/<annex_operator-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "annex_operator": {
      "illegality": "Another illegality for the annex_operator"
  }
}'
```

<aside class="notice">
Remember — create annex_operator is an authenticated endpoint!
</aside>

## Deleting a AnnexOperator
You can delete a annex_operator! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/annex_operators/<annex_operator-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create annex_operator is an authenticated endpoint!
</aside>
