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
              "id": 12,
              "created_at": "2017-04-06T16:24:46.262Z",
              "updated_at": "2017-04-06T16:24:46.277Z",
              "governance_pillar": "Planning and decision making",
              "governance_problem": "Non respect of procedures - attribution of right to exploit, trade or transport CITES species",
              "details": null
            },
            {
              "id": 13,
              "created_at": "2017-04-06T16:24:46.300Z",
              "updated_at": "2017-04-06T16:24:46.317Z",
              "governance_pillar": "Planning and decision making",
              "governance_problem": "Non respect of procedures authorising harvesting of forest resources",
              "details": null
            }
          ]
        },
        "annex_operators": {
          "data": [
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
            },
            {
              "id": 28,
              "country_id": 228,
              "created_at": "2017-04-06T16:24:45.047Z",
              "updated_at": "2017-04-06T16:24:46.885Z",
              "illegality": "Export duty unpaid",
              "details": null
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
              "id": 20,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.644Z",
              "updated_at": "2017-04-06T16:25:18.812Z",
              "illegality": "Operating without a valid license",
              "details": null
            },
            {
              "id": 21,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.692Z",
              "updated_at": "2017-04-06T16:25:17.906Z",
              "illegality": "Harvesting without required permit",
              "details": null
            },
            {
              "id": 22,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.743Z",
              "updated_at": "2017-04-06T16:25:18.740Z",
              "illegality": "Operating without a title",
              "details": null
            },
            {
              "id": 34,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:45.338Z",
              "updated_at": "2017-04-06T16:24:45.354Z",
              "illegality": "Company not registered according to regulations",
              "details": null
            },
            {
              "id": 35,
              "country_id": 102,
              "created_at": "2017-04-06T16:24:45.385Z",
              "updated_at": "2017-04-06T16:25:16.917Z",
              "illegality": "Irregular sub-contracting/transfer of shares",
              "details": null
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
              "id": 3,
              "created_at": "2017-04-06T16:24:45.880Z",
              "updated_at": "2017-04-06T16:24:45.895Z",
              "governance_pillar": "Transparency",
              "governance_problem": "Information not made public as required by law, including the VPA",
              "details": null
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": 3,
              "country_id": 194,
              "created_at": "2017-04-06T16:24:43.778Z",
              "updated_at": "2017-04-06T16:24:53.160Z",
              "illegality": "Insufficient consultation of local/indigenous populations ",
              "details": null
            },
            {
              "id": 16,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.465Z",
              "updated_at": "2017-04-06T16:25:18.304Z",
              "illegality": "Recruitment/management of workers in breach of labour laws ",
              "details": null
            },
            {
              "id": 40,
              "country_id": 102,
              "created_at": "2017-04-06T16:24:45.671Z",
              "updated_at": "2017-04-06T16:25:16.952Z",
              "illegality": "Human rights violation ",
              "details": null
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
              "id": 1,
              "created_at": "2017-04-06T16:24:45.768Z",
              "updated_at": "2017-04-06T16:24:45.792Z",
              "governance_pillar": "Law enforcement",
              "governance_problem": "Corruption leads to illegal activity/poor enforcement",
              "details": null
            },
            {
              "id": 2,
              "created_at": "2017-04-06T16:24:45.838Z",
              "updated_at": "2017-04-06T16:24:45.855Z",
              "governance_pillar": "Law enforcement",
              "governance_problem": "Poor application of sanctions ",
              "details": null
            },
            {
              "id": 4,
              "created_at": "2017-04-06T16:24:45.919Z",
              "updated_at": "2017-04-06T16:24:45.937Z",
              "governance_pillar": "Policy framework",
              "governance_problem": "Policy gaps",
              "details": null
            },
            {
              "id": 5,
              "created_at": "2017-04-06T16:24:45.961Z",
              "updated_at": "2017-04-06T16:24:45.978Z",
              "governance_pillar": "Planning and decision making",
              "governance_problem": "Lack of interagency cooperation ",
              "details": null
            },
            {
              "id": 6,
              "created_at": "2017-04-06T16:24:46.000Z",
              "updated_at": "2017-04-06T16:24:46.016Z",
              "governance_pillar": "Planning and decision making",
              "governance_problem": "Lack of transparency on use of forestry revenues, including taxes and fines",
              "details": null
            },
            {
              "id": 7,
              "created_at": "2017-04-06T16:24:46.039Z",
              "updated_at": "2017-04-06T16:24:46.057Z",
              "governance_pillar": "Law enforcement",
              "governance_problem": "Poor control",
              "details": null
            },
            {
              "id": 8,
              "created_at": "2017-04-06T16:24:46.085Z",
              "updated_at": "2017-04-06T16:24:46.102Z",
              "governance_pillar": "Law enforcement",
              "governance_problem": "Poor reporting of enforcement",
              "details": null
            },
            {
              "id": 10,
              "created_at": "2017-04-06T16:24:46.170Z",
              "updated_at": "2017-04-06T16:24:46.186Z",
              "governance_pillar": "Law enforcement",
              "governance_problem": "Poor distribution of law enforcement means",
              "details": null
            },
            {
              "id": 11,
              "created_at": "2017-04-06T16:24:46.218Z",
              "updated_at": "2017-04-06T16:24:46.237Z",
              "governance_pillar": "Law enforcement",
              "governance_problem": "Non respect of procedures - management of seized goods",
              "details": null
            },
            {
              "id": 14,
              "created_at": "2017-04-06T16:24:46.340Z",
              "updated_at": "2017-04-06T16:24:46.357Z",
              "governance_pillar": "Planning and decision making",
              "governance_problem": "Non respect of procedures authorising transport or export of forest resources",
              "details": null
            },
            {
              "id": 15,
              "created_at": "2017-04-06T16:24:46.380Z",
              "updated_at": "2017-04-06T16:24:46.397Z",
              "governance_pillar": "Planning and decision making",
              "governance_problem": "Non respect of procedures granting access to forest resources",
              "details": null
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": 1,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:43.605Z",
              "updated_at": "2017-04-06T16:25:20.814Z",
              "illegality": "Abandonment of timber ",
              "details": null
            },
            {
              "id": 2,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:43.725Z",
              "updated_at": "2017-04-06T16:25:18.628Z",
              "illegality": "Timber laundering",
              "details": null
            },
            {
              "id": 4,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:43.831Z",
              "updated_at": "2017-04-06T16:25:17.592Z",
              "illegality": "Harvesting non authorised species",
              "details": null
            },
            {
              "id": 5,
              "country_id": 234,
              "created_at": "2017-04-06T16:24:43.909Z",
              "updated_at": "2017-04-06T16:25:17.109Z",
              "illegality": "Harvesting in a protected area or other area where logging is prohibited",
              "details": null
            },
            {
              "id": 6,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:43.992Z",
              "updated_at": "2017-04-06T16:25:17.638Z",
              "illegality": "Cutting outside permit boundaries",
              "details": null
            },
            {
              "id": 7,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.038Z",
              "updated_at": "2017-04-06T16:24:44.059Z",
              "illegality": "Cutting trees below minimum diameter",
              "details": null
            },
            {
              "id": 8,
              "country_id": 53,
              "created_at": "2017-04-06T16:24:44.085Z",
              "updated_at": "2017-04-06T16:24:54.923Z",
              "illegality": "Cutting trees below minimum diameter",
              "details": null
            },
            {
              "id": 10,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.186Z",
              "updated_at": "2017-04-06T16:25:17.216Z",
              "illegality": "Default on markings on logs, stumps, other wood products",
              "details": null
            },
            {
              "id": 11,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.235Z",
              "updated_at": "2017-04-06T16:25:17.749Z",
              "illegality": "Default on demarcation of cutting permit boundaries",
              "details": null
            },
            {
              "id": 14,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.377Z",
              "updated_at": "2017-04-06T16:25:17.800Z",
              "illegality": "Default on maintenance of exploitation documents",
              "details": null
            },
            {
              "id": 15,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.421Z",
              "updated_at": "2017-04-06T16:25:18.261Z",
              "illegality": "Default on transmission of documents to relevant authorities",
              "details": null
            },
            {
              "id": 17,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.510Z",
              "updated_at": "2017-04-06T16:25:17.850Z",
              "illegality": "Overharvesting ",
              "details": null
            },
            {
              "id": 18,
              "country_id": 92,
              "created_at": "2017-04-06T16:24:44.554Z",
              "updated_at": "2017-04-06T16:25:16.346Z",
              "illegality": "Fraudulent behavior ",
              "details": null
            },
            {
              "id": 19,
              "country_id": 53,
              "created_at": "2017-04-06T16:24:44.600Z",
              "updated_at": "2017-04-06T16:25:05.099Z",
              "illegality": "Exploitation or transport of wood outside of authorised timeframe",
              "details": null
            },
            {
              "id": 25,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.900Z",
              "updated_at": "2017-04-06T16:25:17.304Z",
              "illegality": "Non fulfillment of contractual obligations (non socio-economic)",
              "details": null
            },
            {
              "id": 26,
              "country_id": 53,
              "created_at": "2017-04-06T16:24:44.952Z",
              "updated_at": "2017-04-06T16:24:44.969Z",
              "illegality": "Non respect of management plan",
              "details": null
            },
            {
              "id": 30,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:45.148Z",
              "updated_at": "2017-04-06T16:25:17.260Z",
              "illegality": "Non respect of norms for reduced impact logging or environmental regulations",
              "details": null
            },
            {
              "id": 31,
              "country_id": 53,
              "created_at": "2017-04-06T16:24:45.195Z",
              "updated_at": "2017-04-06T16:25:04.357Z",
              "illegality": "Non respect of procedures related to impact assessments or inventories",
              "details": null
            },
            {
              "id": 32,
              "country_id": 51,
              "created_at": "2017-04-06T16:24:45.242Z",
              "updated_at": "2017-04-06T16:24:50.900Z",
              "illegality": "Obstacles to checks by forest law enforcement officials",
              "details": null
            },
            {
              "id": 36,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:45.475Z",
              "updated_at": "2017-04-06T16:24:45.493Z",
              "illegality": "Illegal timber storage",
              "details": null
            },
            {
              "id": 41,
              "country_id": 51,
              "created_at": "2017-04-06T16:24:50.932Z",
              "updated_at": "2017-04-06T16:24:50.932Z",
              "illegality": "Non respect des prescriptions du MINFOF: Les dispositions de la lettre relative aux procédures de délivrance et de suivi d’exécution des petits titres d’exploitation forestière en matière de détermination des emprises n’ont pas été respectées. ",
              "details": null
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
              "id": 9,
              "created_at": "2017-04-06T16:24:46.131Z",
              "updated_at": "2017-04-06T16:24:46.147Z",
              "governance_pillar": "Law enforcement",
              "governance_problem": "Poor tax and fine collection",
              "details": null
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": 9,
              "country_id": 53,
              "created_at": "2017-04-06T16:24:44.136Z",
              "updated_at": "2017-04-06T16:24:44.157Z",
              "illegality": "Default on timber processing documents",
              "details": null
            },
            {
              "id": 37,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:45.524Z",
              "updated_at": "2017-04-06T16:24:45.541Z",
              "illegality": "Processing wood of fraudulent or untraceable origin",
              "details": null
            },
            {
              "id": 38,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:45.572Z",
              "updated_at": "2017-04-06T16:24:45.589Z",
              "illegality": "Processing timber without authorisation",
              "details": null
            },
            {
              "id": 39,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:45.623Z",
              "updated_at": "2017-04-06T16:24:45.642Z",
              "illegality": "Timber processing facility not in place when required ",
              "details": null
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
              "id": 23,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:44.790Z",
              "updated_at": "2017-04-06T16:24:44.810Z",
              "illegality": "Export of CITES species without authorisation",
              "details": null
            },
            {
              "id": 24,
              "country_id": 234,
              "created_at": "2017-04-06T16:24:44.842Z",
              "updated_at": "2017-04-06T16:25:17.033Z",
              "illegality": "Non authorised exportation of timber",
              "details": null
            },
            {
              "id": 27,
              "country_id": 53,
              "created_at": "2017-04-06T16:24:44.998Z",
              "updated_at": "2017-04-06T16:24:45.017Z",
              "illegality": "Non respect of quotas on processed wood",
              "details": null
            },
            {
              "id": 29,
              "country_id": 59,
              "created_at": "2017-04-06T16:24:45.093Z",
              "updated_at": "2017-04-06T16:25:14.809Z",
              "illegality": "Transport regulations breached (registration of vehicle, authorisation of transport...)",
              "details": null
            },
            {
              "id": 33,
              "country_id": 13,
              "created_at": "2017-04-06T16:24:45.290Z",
              "updated_at": "2017-04-06T16:24:45.310Z",
              "illegality": "Origin of timber transported not traceable or timber not identified",
              "details": null
            }
          ]
        }
      }
    }
  ],
  "links": {
    "first": "http://localhost:3000/categories?page%5Bnumber%5D=1",
    "prev": "http://localhost:3000/categories?page%5Bnumber%5D=1",
    "next": "http://localhost:3000/categories?page%5Bnumber%5D=1",
    "last": "http://localhost:3000/categories?page%5Bnumber%5D=1"
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
