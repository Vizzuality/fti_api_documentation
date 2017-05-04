# Observers

## How obtain all observers

To obtain all observers:

```shell
curl -X GET http://localhost:3000/observers \
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
      "id": "3",
      "type": "observers",
      "attributes": {
        "observer_type": "Mandated",
        "name": "AGRECO",
        "organization": "AGRECO",
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
      "id": "12",
      "type": "observers",
      "attributes": {
        "observer_type": "External",
        "name": "Brainforest",
        "organization": "Brainforest",
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
      "id": "10",
      "type": "observers",
      "attributes": {
        "observer_type": "Mandated",
        "name": "CAGDF",
        "organization": "CAGDF",
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
      "id": "4",
      "type": "observers",
      "attributes": {
        "observer_type": "External",
        "name": "CEDLA",
        "organization": "CEDLA",
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
      "id": "9",
      "type": "observers",
      "attributes": {
        "observer_type": "External",
        "name": "CIEDD",
        "organization": "CIEDD",
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
      "id": "13",
      "type": "observers",
      "attributes": {
        "observer_type": "SemiMandated",
        "name": "Conservation Justice",
        "organization": "Conservation Justice",
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
      "id": "16",
      "type": "observers",
      "attributes": {
        "observer_type": "External",
        "name": "CS-IFM",
        "organization": "CS-IFM",
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
      "id": "14",
      "type": "observers",
      "attributes": {
        "observer_type": "External",
        "name": "EIA",
        "organization": "EIA",
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
      "id": "2",
      "type": "observers",
      "attributes": {
        "observer_type": "External",
        "name": "Global Witness",
        "organization": "Global Witness",
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
    }
  ],
  "links": {
    "first": "http://otp-staging.ipq.co/observers?page%5Bnumber%5D=1",
    "prev": "http://otp-staging.ipq.co/observers?page%5Bnumber%5D=1",
    "next": "http://otp-staging.ipq.co/observers?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://otp-staging.ipq.co/observers?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "self": "http://otp-staging.ipq.co/observers?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  },
  "meta": {
    "total_items": 17
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the observers of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/observers?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (name, created_at, updated_at) | Text


> To obtain all observers sorted by name:

```shell
curl -X GET http://localhost:3000/observers?sort=name \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/observers?sort=-name \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific observer

To obtain specific observer:

```shell
curl -X GET http://localhost:3000/observers/33 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a Observer

In order to create a observer, you need an authorization token for current admin.

Only admin should be able to create Observers

To create a observer, you need to define all of the required fields in the request body. The fields that compose a observer are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| name                | Name of the observer                                          | Text    | Any Text                                        | Yes
| observer_type       | Type of observer: Mandated SemiMandated External Government   | Text    | Valid type                                      | No
| country_id          | ID of country                                                 | Integer | Valid country id                                | No
| organization        | Organization of the observer                                  | Text    | Any Text                                        | No
| is_active           | Activate deactiveta observers (only accessible by admin)      | Boolean | default value true                              | No
| logo                | base64 image ({"observer": { "logo": "data:image/jpeg;base64,(/9j/...) }}) | Text    | Valid file base64                  | No

> To create a observer, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/observers \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "observer": {
      "name": "observer Spain",
      "observer_type": "Mandated",
      "logo": "data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wgARCAEsAZADASIAAhEBAxEB/8QAFQABAQAAAAAAAAAAAAAAAAAAAAX/xAAWAQEBAQAAAAAAAAAAAAAAAAAAAwb/2gAMAwEAAhADEAAAAZ4hsgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP/8QAFBABAAAAAAAAAAAAAAAAAAAAoP/aAAgBAQABBQJtn//EABQRAQAAAAAAAAAAAAAAAAAAAID/2gAIAQMBAT8Bbf8A/8QAFBEBAAAAAAAAAAAAAAAAAAAAgP/aAAgBAgEBPwFt/wD/xAAUEAEAAAAAAAAAAAAAAAAAAACg/9oACAEBAAY/Am2f/8QAFBABAAAAAAAAAAAAAAAAAAAAoP/aAAgBAQABPyFtn//aAAwDAQACAAMAAAAQ9999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999//8QAFBEBAAAAAAAAAAAAAAAAAAAAgP/aAAgBAwEBPxBt/wD/xAAUEQEAAAAAAAAAAAAAAAAAAACA/9oACAECAQE/EG3/AP/EABQQAQAAAAAAAAAAAAAAAAAAAKD/2gAIAQEAAT8QbZ//2Q==",
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create observer is an authenticated endpoint!
</aside>


## Updating a Observer

In order to modify the observer, you can PUT/PATCH a request.
It accepts the same parameters as the _create observer_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/observers/<observer-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "observer": {
      "name": "Another name for the observer"
  }
}'
```

<aside class="notice">
Remember — create observer is an authenticated endpoint!
</aside>

## Deleting a Observer
You can delete a observer! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/observers/<observer-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create observer is an authenticated endpoint!
</aside>
