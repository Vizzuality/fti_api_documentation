# Observations

## How obtain all observations

To obtain all observations:

```shell
curl -X GET http://localhost:3000/observations \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>

> Example response:

```json
{
  "data": {
    "id": "33",
    "type": "observations",
    "attributes": {
      "observation_type": "AnnexOperator",
      "publication_date": "0002-01-16T00:00:00.000Z",
      "pv": null,
      "is_active": true,
      "details": "GSE bénéfice uniquement de bois déjà abattus, abandonnés et stockés depuis 2011 dans les anciens parcs de l’entreprise COMOCA ; enlève plutôt des bois abattus beaucoup plus récemment. En effet, les dates marquées sur certaines billes de bois observées par la mission, démontrent que les bois ont été abattus aux mois de novembre 2015 et janvier 2016.",
      "evidence": null,
      "concern_opinion": null,
      "litigation_status": null
    },
    "relationships": {
      "country": {
        "data": {
          "id": "45",
          "type": "countries"
        }
      },
      "annex_operator": {
        "data": {
          "id": "22",
          "type": "annex_operators"
        }
      },
      "annex_governance": {
        "data": null
      },
      "severity": {
        "data": {
          "id": "85",
          "type": "severities"
        }
      },
      "user": {
        "data": null
      },
      "observer": {
        "data": {
          "id": "5",
          "type": "observers"
        }
      },
      "operator": {
        "data": {
          "id": "20",
          "type": "operators"
        }
      },
      "government": {
        "data": null
      },
      "species": {
        "data": []
      },
      "comments": {
        "data": []
      },
      "photos": {
        "data": []
      },
      "documents": {
        "data": [
          {
            "id": "33",
            "type": "documents"
          }
        ]
      }
    }
  },
  "included": [
    {
      "id": "45",
      "type": "countries",
      "attributes": {
        "iso": "CMR",
        "region_iso": "MA",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            6,
            12.5
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            0.618107263658459,
            19.464922564119
          ]
        },
        "is_active": true,
        "name": "Cameroon",
        "region_name": "Middle Africa"
      }
    },
    {
      "id": "22",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Operating without a title",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "85",
              "type": "severities"
            },
            {
              "id": "86",
              "type": "severities"
            },
            {
              "id": "87",
              "type": "severities"
            },
            {
              "id": "88",
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
          "data": [
            {
              "id": "38",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "85",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "5",
      "type": "observers",
      "attributes": {
        "observer_type": "SemiMandated",
        "name": "FODER",
        "organization": "FODER",
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
        }
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
      "id": "20",
      "type": "operators",
      "attributes": {
        "name": "Grandes Scieries d'Edéa",
        "operator_type": "Sawmill",
        "concession": "Convention de Vente aux Enchères Publics de Bois)",
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
      "id": "33",
      "type": "documents",
      "attributes": {
        "name": "2016 Rapport Fev FODER",
        "attachment": {
          "url": null
        },
        "document_type": "Report",
        "user_id": null
      },
      "relationships": {
        "attacheable": {
          "data": {
            "id": "33",
            "type": "observations"
          }
        }
      }
    }
  ],
  "meta": {
    "updated_at": "2017-04-24T15:35:02.425Z",
    "created_at": "2017-04-24T15:35:02.408Z"
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the observations of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/observations?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (evidence, created_at, updated_at) | Text


> To obtain all observations sorted by evidence:

```shell
curl -X GET http://localhost:3000/observations?sort=evidence \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/observations?sort=-evidence \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific observation

To obtain specific observation:

```shell
curl -X GET http://localhost:3000/observations/33 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a Observation

In order to create a observation, you need an authorization token for current admin or ngo user.

Only admin or ngo user should be able to create Observations

To create a observation, you need to define all of the required fields in the request body. The fields that compose a observation are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| evidence            | Evidence of the observation                                   | Text    | Any Text                                       | No
| observation_type    | Type of observation: AnnexGovernance AnnexOperator            | Text    | Valid type                                     | Yes
| country_id          | ID of country                                                 | Integer | Valid country id                               | Yes
| details             | Description of the observation                                | Text    | Any Text                                       | No
| concern_opinion     | Operator's opinion                                            | Text    | Any Text                                       | No
| litigation_status   | Litigation status of the observation                          | Text    | Any Text                                       | No
| pv                  | PV of the observation                                         | Text    | Any Text                                       | No
| annex_operator_id   | ID of operator                                                | Integer | Valid operator id                              | No
| annex_governance_id | ID of governance                                              | Integer | Valid governance id                            | No
| severity_id         | ID of severity                                                | Integer | Valid severity id                              | No
| user_id             | ID of user (default current_user)                             | Integer | Valid user id                                  | No
| observer_id         | ID of observer/monitor                                        | Integer | Valid observer id                              | No
| operator_id         | ID of operator/company                                        | Integer | Valid operator id                              | No
| government_id       | ID of government                                              | Integer | Valid government id                            | No
| publication_date    | Date of publication                                           | Date    | Date time                                      | Yes
| is_active           | Activate deactiveta observations (only accessible by admin)   | Boolean | default value true                             | No
| photos_attributes   | base64 image ({"observation": { "photos_attributes": [{"name": "observation photo", "attachment": "data:image/jpeg;base64,(/9j/...)" }] }}) | Array    | Valid file base64                  | No
| documents_attributes   | base64 document ({"observation": { "documents_attributes": [{"name": "observation document", "attachment": "data:application/pdf;base64,(/9j/...)" }] }}) | Array    | Valid file base64                  | No
| available photos_attributes   | { photos_attributes: [:id, :name, :attachment, :user_id, :_destroy] }   | Array |                             | No
| available documents_attributes   | { documents_attributes: [:id, :name, :attachment, :document_type, :user_id, :_destroy] }   | Array |                             | No

> To create a observation, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/observations \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "observation": {
      "evidence": "observation Spain",
      "observation_type": "AnnexOperator",
      "photos_attributes": [{"name": "test photo", "data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wgARCAEsAZADASIAAhEBAxEB/8QAFQABAQAAAAAAAAAAAAAAAAAAAAX/xAAWAQEBAQAAAAAAAAAAAAAAAAAAAwb/2gAMAwEAAhADEAAAAZ4hsgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP/8QAFBABAAAAAAAAAAAAAAAAAAAAoP/aAAgBAQABBQJtn//EABQRAQAAAAAAAAAAAAAAAAAAAID/2gAIAQMBAT8Bbf8A/8QAFBEBAAAAAAAAAAAAAAAAAAAAgP/aAAgBAgEBPwFt/wD/xAAUEAEAAAAAAAAAAAAAAAAAAACg/9oACAEBAAY/Am2f/8QAFBABAAAAAAAAAAAAAAAAAAAAoP/aAAgBAQABPyFtn//aAAwDAQACAAMAAAAQ9999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999//8QAFBEBAAAAAAAAAAAAAAAAAAAAgP/aAAgBAwEBPxBt/wD/xAAUEQEAAAAAAAAAAAAAAAAAAACA/9oACAECAQE/EG3/AP/EABQQAQAAAAAAAAAAAAAAAAAAAKD/2gAIAQEAAT8QbZ//2Q=="}],
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create observation is an authenticated endpoint!
</aside>


## Updating a Observation

In order to modify the observation, you can PUT/PATCH a request.
It accepts the same parameters as the _create observation_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/observations/<observation-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "observation": {
      "evidence": "Another evidence for the observation",
      "photos_attributes": [{"id": <photo-id>,"name": "test photo update with new photo", "data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wgARCAEsAZADASIAAhEBAxEB/8QAFQABAQAAAAAAAAAAAAAAAAAAAAX/xAAWAQEBAQAAAAAAAAAAAAAAAAAAAwb/2gAMAwEAAhADEAAAAZ4hsgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP/8QAFBABAAAAAAAAAAAAAAAAAAAAoP/aAAgBAQABBQJtn//EABQRAQAAAAAAAAAAAAAAAAAAAID/2gAIAQMBAT8Bbf8A/8QAFBEBAAAAAAAAAAAAAAAAAAAAgP/aAAgBAgEBPwFt/wD/xAAUEAEAAAAAAAAAAAAAAAAAAACg/9oACAEBAAY/Am2f/8QAFBABAAAAAAAAAAAAAAAAAAAAoP/aAAgBAQABPyFtn//aAAwDAQACAAMAAAAQ9999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999//8QAFBEBAAAAAAAAAAAAAAAAAAAAgP/aAAgBAwEBPxBt/wD/xAAUEQEAAAAAAAAAAAAAAAAAAACA/9oACAECAQE/EG3/AP/EABQQAQAAAAAAAAAAAAAAAAAAAKD/2gAIAQEAAT8QbZ//2Q=="}]
  }
}'
```

<aside class="notice">
Remember — create observation is an authenticated endpoint!
</aside>

## Deleting a Observation
You can delete a observation! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/observations/<observation-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create observation is an authenticated endpoint!
</aside>

## Deleting a attachment (Photo/document) from Observation
You can delete a observation's photo! Just send a patch request to the endpoint:

```shell
curl -X PATCH http://localhost:3000/observations/<observation-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "observation": {
      "photos_attributes": [{"id": <photo-id>,"_detroy": true}]
  }
}'
```

<aside class="notice">
Remember — create observation is an authenticated endpoint!
</aside>
