# Laws

## How obtain all laws

To obtain all laws:

```shell
curl -X GET http://localhost:3000/laws \
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
      "id": "161",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 119 al 2 et 123 al 1",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "153",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 158 et 159 de la loi forestière de 1994",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "155",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 159 et 163 de la loi forestière",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "164",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 168",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "121",
      "type": "laws",
      "attributes": {
        "vpa_indicator": "2.1.2 The permit holder can demonstrate that the transported logs are from areas under valid land conversion  permit/ other use permits (IPK/ILS)",
        "legal_reference": "2009 Environmental Law",
        "legal_penalty": " "
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "201",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 23 arrêté rministériel 035 (valable jusqu'en 2015); Art. 97 code forestier et Art. 11 arrêté 035/2006; Art.145 code foretier (falsificaiton d'agrement)-Article 8 et 9 de l'arrêté 084/2016 portant conditions et règles d'exploitation de bois d'oeuvre (valable depuis octobre 2016)",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "197",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 2 et 3 de l’arrêté interministériel n° 002/2013 et n° 924/2013 du 05/8/2013 portant fixation des taux",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "188",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 49 arrêté 035/2006 (abrogé en 2015)-Article 66 de l'arrêté 084/2016 portant conditions et règles d'exploitation de bois d'oeuvre -valable depuis octobre 2016)",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "148",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 53 et 54 de la loi 94/01 du 20 janvier 1994 portant régime des forêts",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "175",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 67 et Décret 2002-437 Art. 68 al 2",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    }
  ],
  "links": {
    "first": "http://otp-staging.ipq.co/laws?page%5Bnumber%5D=1",
    "prev": "http://otp-staging.ipq.co/laws?page%5Bnumber%5D=1",
    "next": "http://otp-staging.ipq.co/laws?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://otp-staging.ipq.co/laws?page%5Bnumber%5D=21&page%5Bsize%5D=10",
    "self": "http://otp-staging.ipq.co/laws?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  },
  "meta": {
    "total_items": 203
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the laws of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/laws?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (legal_reference, created_at, updated_at) | Text
| country       | Filter by country ID | Integer


> To obtain all laws sorted by legal_reference:

```shell
curl -X GET http://localhost:3000/laws?sort=legal_reference \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/laws?sort=-legal_reference \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

> To filter laws by specific country:

```shell
curl -X GET http://localhost:3000/laws?country=<country-id> \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific law

To obtain specific law:

```shell
curl -X GET http://localhost:3000/laws/33 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a Law

In order to create a law, you need an authorization token for current admin.

Only admin should be able to create Laws

To create a law, you need to define all of the required fields in the request body. The fields that compose a law are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| legal_reference     | Name of the law                                               | Text    | Any Text                                        | Yes
| legal_penalty       | Name of penalty                                               | Text    | Any Text                                        | No
| country_id          | ID of country                                                 | Integer | Valid country id                                | No
| vpa_indicator       | VPA indicator of the law                                      | Text    | Any Text                                        | No

> To create a law, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/laws \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "law": {
      "legal_reference": "Spain",
      "legal_penalty": "ESP",
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create law is an authenticated endpoint!
</aside>


## Updating a Law

In order to modify the law, you can PUT/PATCH a request.
It accepts the same parameters as the _create law_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/laws/<law-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "law": {
      "legal_reference": "Another legal_reference for the law"
  }
}'
```

<aside class="notice">
Remember — create law is an authenticated endpoint!
</aside>

## Deleting a Law
You can delete a law! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/laws/<law-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create law is an authenticated endpoint!
</aside>
