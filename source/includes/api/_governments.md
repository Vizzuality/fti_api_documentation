# Governments

## How obtain all governments

To obtain all governments:

```shell
curl -X GET http://localhost:3000/governments \
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
      "id": "12",
      "type": "governments",
      "attributes": {
        "government_entity": "CIMA - Commission interministérielle d’attribution",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "194",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "58",
      "type": "governments",
      "attributes": {
        "government_entity": "Chef Unité de Gestion Forestière",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "92",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "55",
      "type": "governments",
      "attributes": {
        "government_entity": "Chief of police in Lamandau",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "36",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "6",
      "type": "governments",
      "attributes": {
        "government_entity": "Customs & Excise Agency",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "228",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "46",
      "type": "governments",
      "attributes": {
        "government_entity": "DCVI",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "13",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "52",
      "type": "governments",
      "attributes": {
        "government_entity": "DCVI du MECNT",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "13",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "25",
      "type": "governments",
      "attributes": {
        "government_entity": "DDEF-Bouenza, DDEF-Lék, DDEF-Nairi",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "53",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "16",
      "type": "governments",
      "attributes": {
        "government_entity": "DDEF-CO",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "53",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "20",
      "type": "governments",
      "attributes": {
        "government_entity": "DDEF-Cu",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "53",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "30",
      "type": "governments",
      "attributes": {
        "government_entity": "DDEF-Cuvette",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "53",
            "type": "countries"
          }
        }
      }
    }
  ],
  "links": {
    "first": "http://localhost:3000/governments?page%5Bnumber%5D=1",
    "prev": "http://localhost:3000/governments?page%5Bnumber%5D=1",
    "next": "http://localhost:3000/governments?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://localhost:3000/governments?page%5Bnumber%5D=7&page%5Bsize%5D=10",
    "self": "http://localhost:3000/governments?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the governments of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/governments?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (government_entity, created_at, updated_at) | Text


> To obtain all governments sorted by government_entity:

```shell
curl -X GET http://localhost:3000/governments?sort=government_entity \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/governments?sort=-government_entity \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific government

To obtain specific government:

```shell
curl -X GET http://localhost:3000/governments/33 \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a Government

In order to create a government, you need an authorization token for current admin.

Only admin should be able to create Governments

To create a government, you need to define all of the required fields in the request body. The fields that compose a government are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| government_entity   | Name of the government                                        | Text    | Any Text                                        | Yes
| country_id          | ID of country                                                 | Integer | Valid country id                                | No
| details             | Details - description                                         | Text    | Any Text                                        | No

> To create a government, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/governments \
-H "Authorization: Bearer <your-token>" \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "government": {
      "government_entity": "Spain",
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create government is an authenticated endpoint!
</aside>


## Updating a Government

In order to modify the government, you can PUT/PATCH a request.
It accepts the same parameters as the _create government_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/governments/<government-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "government": {
      "government_entity": "Another government_entity for the government"
  }
}'
```

<aside class="notice">
Remember — create government is an authenticated endpoint!
</aside>

## Deleting a Government
You can delete a government! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/governments/<government-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create government is an authenticated endpoint!
</aside>
