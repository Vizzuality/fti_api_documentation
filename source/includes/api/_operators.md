# Operators

## How obtain all operators

To obtain all operators:

```shell
curl -X GET http://localhost:3000/operators \
-H "OTP_API_KEY: Bearer <your-api-key>" \
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
      "id": "219",
      "type": "operators",
      "attributes": {
        "name": "ACI",
        "operator_type": "Company",
        "concession": null,
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "241",
      "type": "operators",
      "attributes": {
        "name": "ACI, CIBN",
        "operator_type": "Company",
        "concession": null,
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "256",
      "type": "operators",
      "attributes": {
        "name": "ACI, CIBN, FORALAC, SFIBet TAMAN",
        "operator_type": "Company",
        "concession": null,
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "237",
      "type": "operators",
      "attributes": {
        "name": "ACI, FOROLAC",
        "operator_type": "Company",
        "concession": null,
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "236",
      "type": "operators",
      "attributes": {
        "name": "ACI, SFIB",
        "operator_type": "Company",
        "concession": null,
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "242",
      "type": "operators",
      "attributes": {
        "name": "ACI, SICOFOR",
        "operator_type": "Company",
        "concession": null,
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "244",
      "type": "operators",
      "attributes": {
        "name": "ACI, SICOFOR, TAMAN et FORALAC",
        "operator_type": "Company",
        "concession": null,
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "100",
      "type": "operators",
      "attributes": {
        "name": "ADL",
        "operator_type": "Logging Company",
        "concession": "MOUYALA",
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "27",
      "type": "operators",
      "attributes": {
        "name": "AFRIGRUM",
        "operator_type": "Logging Company",
        "concession": "VC 08 06 156",
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    },
    {
      "id": "106",
      "type": "operators",
      "attributes": {
        "name": "ASIA CONGO INDUSTRIE",
        "operator_type": "Logging Company",
        "concession": "Ngongo-Nzambi",
        "is_active": true,
        "logo": {
          "url": "/placeholder.png",
          "thumbnail": {
            "url": "/thumbnail_placeholder.png"
          },
          "square": {
            "url": "/square_placeholder.png"
          },
          "medium": {
            "url": "/medium_placeholder.png"
          }
        },
        "details": null
      },
      "relationships": {
        "country": {
          "data": null
        },
        "users": {
          "data": []
        }
      }
    }
  ],
  "links": {
    "first": "http://localhost:3000/operators?page%5Bnumber%5D=1",
    "prev": "http://localhost:3000/operators?page%5Bnumber%5D=1",
    "next": "http://localhost:3000/operators?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://localhost:3000/operators?page%5Bnumber%5D=27&page%5Bsize%5D=10",
    "self": "http://localhost:3000/operators?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the operators of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/operators?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (name, created_at, updated_at) | Text


> To obtain all operators sorted by name:

```shell
curl -X GET http://localhost:3000/operators?sort=name \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/operators?sort=-name \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific operator

To obtain specific operator:

```shell
curl -X GET http://localhost:3000/operators/33 \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a Operator

In order to create a operator, you need an authorization token for current admin.

Only admin should be able to create Operators

To create a operator, you need to define all of the required fields in the request body. The fields that compose a operator are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| name                | Name of the operator                                          | Text    | Any Text                                        | Yes
| operator_type       | Type of operator: Logging Company, Artisanal, Sawmill, CommunityForest, ARB1327, PalmOil, Trader , Company           | Text    | Valid type                                      | No
| country_id          | ID of country                                                 | Integer | Valid country id                                | No
| concession          | Concession of the operator                                    | Text    | Any Text                                        | No
| is_active           | Activate deactiveta operators (only accessible by admin)      | Boolean | default value true                              | No
| logo                | Path to image                                                 | Text    | Valid file path                                 | No
| details             | Datails - description                                         | Text    | Any Text                                        | No
| country_ids         | ID's of countries                                             | Array   | Valid countries ids array                       | No


> To create a operator, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/operators \
-H "Authorization: Bearer <your-token>" \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "operator": {
      "name": "operator Spain",
      "details": "Lorem ipsum...",
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create operator is an authenticated endpoint!
</aside>


## Updating a Operator

In order to modify the operator, you can PUT/PATCH a request.
It accepts the same parameters as the _create operator_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/operators/<operator-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "operator": {
      "name": "Another name for the operator"
  }
}'
```

<aside class="notice">
Remember — create operator is an authenticated endpoint!
</aside>

## Deleting a Operator
You can delete a operator! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/operators/<operator-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create operator is an authenticated endpoint!
</aside>
