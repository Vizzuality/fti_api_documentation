# AnnexGovernances

## How obtain all annex_governances

To obtain all annex_governances:

```shell
curl -X GET http://localhost:3000/annex_governances \
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
      "id": "10",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Law enforcement",
        "governance_problem": "Poor distribution of law enforcement means",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "199",
              "type": "severities"
            },
            {
              "id": "200",
              "type": "severities"
            },
            {
              "id": "198",
              "type": "severities"
            },
            {
              "id": "197",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "1",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Law enforcement",
        "governance_problem": "Corruption leads to illegal activity/poor enforcement",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "164",
              "type": "severities"
            },
            {
              "id": "163",
              "type": "severities"
            },
            {
              "id": "162",
              "type": "severities"
            },
            {
              "id": "161",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "2",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Law enforcement",
        "governance_problem": "Poor application of sanctions ",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "168",
              "type": "severities"
            },
            {
              "id": "167",
              "type": "severities"
            },
            {
              "id": "166",
              "type": "severities"
            },
            {
              "id": "165",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "9",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Law enforcement",
        "governance_problem": "Poor tax and fine collection",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "196",
              "type": "severities"
            },
            {
              "id": "195",
              "type": "severities"
            },
            {
              "id": "194",
              "type": "severities"
            },
            {
              "id": "193",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "11",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Law enforcement",
        "governance_problem": "Non respect of procedures - management of seized goods",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "204",
              "type": "severities"
            },
            {
              "id": "203",
              "type": "severities"
            },
            {
              "id": "202",
              "type": "severities"
            },
            {
              "id": "201",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "7",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Law enforcement",
        "governance_problem": "Poor control",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "188",
              "type": "severities"
            },
            {
              "id": "187",
              "type": "severities"
            },
            {
              "id": "186",
              "type": "severities"
            },
            {
              "id": "185",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "8",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Law enforcement",
        "governance_problem": "Poor reporting of enforcement",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "192",
              "type": "severities"
            },
            {
              "id": "191",
              "type": "severities"
            },
            {
              "id": "190",
              "type": "severities"
            },
            {
              "id": "189",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "5",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Planning and decision making",
        "governance_problem": "Lack of interagency cooperation ",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "180",
              "type": "severities"
            },
            {
              "id": "179",
              "type": "severities"
            },
            {
              "id": "178",
              "type": "severities"
            },
            {
              "id": "177",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "6",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Planning and decision making",
        "governance_problem": "Lack of transparency on use of forestry revenues, including taxes and fines",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "184",
              "type": "severities"
            },
            {
              "id": "183",
              "type": "severities"
            },
            {
              "id": "182",
              "type": "severities"
            },
            {
              "id": "181",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    },
    {
      "id": "12",
      "type": "annex_governances",
      "attributes": {
        "governance_pillar": "Planning and decision making",
        "governance_problem": "Non respect of procedures - attribution of right to exploit, trade or transport CITES species",
        "details": null
      },
      "relationships": {
        "severities": {
          "data": [
            {
              "id": "208",
              "type": "severities"
            },
            {
              "id": "207",
              "type": "severities"
            },
            {
              "id": "206",
              "type": "severities"
            },
            {
              "id": "205",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": []
        },
        "comments": {
          "data": []
        }
      }
    }
  ],
  "included": [
    {
      "id": "199",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "200",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "198",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "197",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "164",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "163",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "162",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "161",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "168",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "167",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "166",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "165",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "196",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "195",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "194",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "193",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "204",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "203",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "202",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "201",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "188",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "187",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "186",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "185",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "192",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "191",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "190",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "189",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "180",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "179",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "178",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "177",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "184",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "183",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "182",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "181",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "208",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "207",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "206",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "205",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    }
  ],
  "links": {
    "first": "http://otp-staging.ipq.co/annex_governances?page%5Bnumber%5D=1",
    "prev": "http://otp-staging.ipq.co/annex_governances?page%5Bnumber%5D=1",
    "next": "http://otp-staging.ipq.co/annex_governances?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://otp-staging.ipq.co/annex_governances?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "self": "http://otp-staging.ipq.co/annex_governances?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  },
  "meta": {
    "total_items": 15
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the annex_governances of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/annex_governances?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (governance_pillar, created_at, updated_at) | Text


> To obtain all annex_governances sorted by governance_pillar:

```shell
curl -X GET http://localhost:3000/annex_governances?sort=governance_pillar \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/annex_governances?sort=-governance_pillar \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific annex_governance

To obtain specific annex_governance:

```shell
curl -X GET http://localhost:3000/annex_governances/33 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a AnnexGovernance

In order to create a annex_governance, you need an authorization token for current admin.

Only admin should be able to create AnnexGovernances

To create a annex_governance, you need to define all of the required fields in the request body. The fields that compose a annex_governance are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| governance_pillar   | Name of the annex_governance                                  | Text    | Any Text                                        | Yes
| governance_problem  | Name of problem                                               | Text    | Any Text                                        | Yes
| details             | Datails - description                                         | Text    | Any Text                                        | No
| category_ids        | ID's of categories                                            | Array   | Valid category ids                              | No
| severities_attributes | Nested severities attributes. Sample: "severities_attributes": [{ "level": 2, "details": "Lorem ipsum" }, { "id": 2, "details": "Lorem ipsum update details for severity id 2" }]                               | Array   | Valid array of object (Severity)    | No


> To create a annex_governance, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/annex_governances \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "annex_governance": {
      "governance_pillar": "Art. 100",
      "governance_problem": "Problem",
      "severities_attributes": [{ "level": 2, "details": "Lorem ipsum" }, { "id": 2, "details": "Lorem ipsum update details for severity id 2" }],
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create annex_governance is an authenticated endpoint!
</aside>


## Updating a AnnexGovernance

In order to modify the annex_governance, you can PUT/PATCH a request.
It accepts the same parameters as the _create annex_governance_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/annex_governances/<annex_governance-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "annex_governance": {
      "governance_pillar": "Another governance_pillar for the annex_governance"
  }
}'
```

<aside class="notice">
Remember — create annex_governance is an authenticated endpoint!
</aside>

## Deleting a AnnexGovernance
You can delete a annex_governance! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/annex_governances/<annex_governance-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create annex_governance is an authenticated endpoint!
</aside>
