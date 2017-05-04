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
  "data": [
    {
      "id": "693",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0010-01-16T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "La société SODEFOR/ Nteno est redevable de la somme de 76 912 000 CDF soit 83 600 USD au trésor public à titre de redevance de superficie forestière pour les exercices 2013 et 2014.",
        "evidence": "Company document",
        "concern_opinion": null,
        "litigation_status": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "annex_operator": {
          "data": {
            "id": "13",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "50",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "17",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "191",
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
              "id": "693",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "438",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0006-01-13T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Mauvaise tenue des documents de chantier 45actérisée par le non enregistrement de certains arbres: plusieurs grumes sont évacuées, transformées ou même exportées sans que leurs spécifications n’aient été consignées dans le 45net de chantier.",
        "evidence": "Company document",
        "concern_opinion": null,
        "litigation_status": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        },
        "annex_operator": {
          "data": {
            "id": "14",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "54",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "11",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "114",
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
              "id": "438",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "447",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0006-01-13T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Indice de dépassement du nombre de pieds autorisé pour certaines essences: la présence de certaines essences parmi les bois d’éclairage route n’ayant pas été répertoriés lors du comptage systématique est un indicateur du non respect des règles qui encadrent la réalisation de cette opération",
        "evidence": "Company document",
        "concern_opinion": null,
        "litigation_status": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        },
        "annex_operator": {
          "data": {
            "id": "17",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "68",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "11",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "139",
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
              "id": "447",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "156",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0002-01-08T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Actes de faux et usage de faux: des documents édités au nom de l'AEB 221, qui n'existe pas, et portant des numéros identiques à ceux de l'AEB 1102 ont été utilisés pour transporter des bois illégalement exploités.",
        "evidence": "Company document",
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
            "id": "18",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "69",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "8",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "84",
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
              "id": "156",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "69",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0006-01-07T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Evacuation de bois exploités en 2006 avec les les lettres de voitures de l'exercice 2007",
        "evidence": "Company document",
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
            "id": "24",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "94",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "8",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "41",
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
              "id": "69",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "463",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0002-01-13T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Coupe en sus de 34 pieds de Doussié bip dans le bloc 1",
        "evidence": "Company document",
        "concern_opinion": null,
        "litigation_status": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        },
        "annex_operator": {
          "data": {
            "id": "17",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "67",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "11",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "117",
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
              "id": "463",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "467",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0002-01-13T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Pour plusieurs arbres abattus figurant dans les 45nets de chantier, les données permettant de calculer la taxe d’abattage ne sont pas disponibles, alors que les billes qui en sont issues ont été évacuées et même exportées pour certaines",
        "evidence": "Company document",
        "concern_opinion": null,
        "litigation_status": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        },
        "annex_operator": {
          "data": {
            "id": "18",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "72",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "11",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "117",
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
              "id": "467",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "648",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0010-01-16T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Cette société reste redevable de 161 214 831,4 CDF (175 233,51 USD) au trésor public à titre de redevance de superficie forestière pour les exercices 2012, 2013 et 2014",
        "evidence": "Company document",
        "concern_opinion": null,
        "litigation_status": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "annex_operator": {
          "data": {
            "id": "13",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "49",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "17",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "180",
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
              "id": "648",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "342",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0010-01-11T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Non mise à jour des 45nets de chantier",
        "evidence": "Company document",
        "concern_opinion": null,
        "litigation_status": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        },
        "annex_operator": {
          "data": {
            "id": "14",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "55",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "11",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "101",
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
              "id": "342",
              "type": "documents"
            }
          ]
        }
      }
    },
    {
      "id": "522",
      "type": "observations",
      "attributes": {
        "observation_type": "AnnexOperator",
        "publication_date": "0002-01-13T00:00:00.000Z",
        "pv": null,
        "is_active": true,
        "details": "Coupe sous diamètre des pieds d'okoumé: pieds d’okoumé ayant un diamètre à la base compris entre 60 et 65 cm ont été exploités par la société TIL.",
        "evidence": "Company document",
        "concern_opinion": null,
        "litigation_status": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        },
        "annex_operator": {
          "data": {
            "id": "8",
            "type": "annex_operators"
          }
        },
        "annex_governance": {
          "data": null
        },
        "severity": {
          "data": {
            "id": "32",
            "type": "severities"
          }
        },
        "user": {
          "data": null
        },
        "observer": {
          "data": {
            "id": "11",
            "type": "observers"
          }
        },
        "operator": {
          "data": {
            "id": "123",
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
              "id": "522",
              "type": "documents"
            }
          ]
        }
      }
    }
  ],
  "links": {
    "first": "http://otp-staging.ipq.co/observations?page%5Bnumber%5D=1",
    "prev": "http://otp-staging.ipq.co/observations?page%5Bnumber%5D=1",
    "next": "http://otp-staging.ipq.co/observations?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://otp-staging.ipq.co/observations?page%5Bnumber%5D=111&page%5Bsize%5D=10",
    "self": "http://otp-staging.ipq.co/observations?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  },
  "meta": {
    "total_items": 1102
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
| type          | filter by observation's type (governance, operator)                          | Text
| user          | filter by user (current (by current user), user_id (by specific user), none (all)) | Text
| country       | Filter by country ID | Integer


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

> To obtain all observations by type operator:

```shell
curl -X GET http://localhost:3000/observations?type=operator \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

> To obtain all observations by type governance:

```shell
curl -X GET http://localhost:3000/observations?type=governance \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

> To obtain all observations by current user:

```shell
curl -X GET http://localhost:3000/observations?user=current \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

> To obtain all observations by specific user:

```shell
curl -X GET http://localhost:3000/observations?user=2 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

> To obtain all observations by all users:

```shell
curl -X GET http://localhost:3000/observations?user=none \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

> To filter observations by specific country:

```shell
curl -X GET http://localhost:3000/observations?country=<country-id> \
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
