# Species

## How obtain all species

To obtain all species:

```shell
curl -X GET http://localhost:3000/species \
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
      "id": "2826",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "abbotti",
        "species_class": "Reptilia",
        "sub_species": "Phelsuma abbotti",
        "species_family": "Gekkonidae",
        "species_kingdom": "Animalia",
        "scientific_name": "Stejneger, 1893",
        "cites_status": "II",
        "cites_id": 5735,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": [
            {
              "id": "228",
              "type": "countries"
            },
            {
              "id": "202",
              "type": "countries"
            }
          ]
        }
      }
    },
    {
      "id": "1911",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "abbotti",
        "species_class": "Aves",
        "sub_species": "Papasula abbotti",
        "species_family": "Sulidae",
        "species_kingdom": "Animalia",
        "scientific_name": "Ridgway, 1893",
        "cites_status": "I",
        "cites_id": 6600,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": [
            {
              "id": "159",
              "type": "countries"
            },
            {
              "id": "30",
              "type": "countries"
            },
            {
              "id": "1",
              "type": "countries"
            }
          ]
        }
      }
    },
    {
      "id": "3732",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "abbreviata",
        "species_class": "Gastropoda",
        "sub_species": "Achatinella abbreviata",
        "species_family": "Achatinellidae",
        "species_kingdom": "Animalia",
        "scientific_name": "Reeve, 1850",
        "cites_status": "I",
        "cites_id": 6788,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "4918",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "abdita",
        "species_class": "Anthozoa",
        "sub_species": "Favites abdita",
        "species_family": "Faviidae",
        "species_kingdom": "Animalia",
        "scientific_name": "(Ellis & Solander, 1786)",
        "cites_status": "II",
        "cites_id": 9294,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": [
            {
              "id": "228",
              "type": "countries"
            },
            {
              "id": "227",
              "type": "countries"
            },
            {
              "id": "211",
              "type": "countries"
            },
            {
              "id": "208",
              "type": "countries"
            },
            {
              "id": "207",
              "type": "countries"
            },
            {
              "id": "205",
              "type": "countries"
            },
            {
              "id": "203",
              "type": "countries"
            },
            {
              "id": "202",
              "type": "countries"
            },
            {
              "id": "195",
              "type": "countries"
            },
            {
              "id": "194",
              "type": "countries"
            },
            {
              "id": "193",
              "type": "countries"
            },
            {
              "id": "178",
              "type": "countries"
            },
            {
              "id": "171",
              "type": "countries"
            },
            {
              "id": "160",
              "type": "countries"
            },
            {
              "id": "158",
              "type": "countries"
            },
            {
              "id": "146",
              "type": "countries"
            },
            {
              "id": "142",
              "type": "countries"
            },
            {
              "id": "138",
              "type": "countries"
            },
            {
              "id": "134",
              "type": "countries"
            },
            {
              "id": "123",
              "type": "countries"
            },
            {
              "id": "122",
              "type": "countries"
            },
            {
              "id": "116",
              "type": "countries"
            },
            {
              "id": "109",
              "type": "countries"
            },
            {
              "id": "107",
              "type": "countries"
            },
            {
              "id": "102",
              "type": "countries"
            },
            {
              "id": "93",
              "type": "countries"
            },
            {
              "id": "77",
              "type": "countries"
            },
            {
              "id": "72",
              "type": "countries"
            },
            {
              "id": "69",
              "type": "countries"
            },
            {
              "id": "67",
              "type": "countries"
            },
            {
              "id": "65",
              "type": "countries"
            },
            {
              "id": "63",
              "type": "countries"
            },
            {
              "id": "59",
              "type": "countries"
            },
            {
              "id": "57",
              "type": "countries"
            },
            {
              "id": "55",
              "type": "countries"
            },
            {
              "id": "51",
              "type": "countries"
            },
            {
              "id": "49",
              "type": "countries"
            },
            {
              "id": "42",
              "type": "countries"
            },
            {
              "id": "30",
              "type": "countries"
            },
            {
              "id": "25",
              "type": "countries"
            },
            {
              "id": "21",
              "type": "countries"
            },
            {
              "id": "1",
              "type": "countries"
            }
          ]
        }
      }
    },
    {
      "id": "3441",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "abditus",
        "species_class": "Amphibia",
        "sub_species": "Andinobates abditus",
        "species_family": "Dendrobatidae",
        "species_kingdom": "Animalia",
        "scientific_name": "(Myers & Daly, 1976)",
        "cites_status": "II",
        "cites_id": 4231,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": [
            {
              "id": "87",
              "type": "countries"
            }
          ]
        }
      }
    },
    {
      "id": "49",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "abdominalis",
        "species_class": "Actinopteri",
        "sub_species": "Hippocampus abdominalis",
        "species_family": "Syngnathidae",
        "species_kingdom": "Animalia",
        "scientific_name": "Lesson, 1827",
        "cites_status": "II",
        "cites_id": 6480,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": [
            {
              "id": "19",
              "type": "countries"
            },
            {
              "id": "1",
              "type": "countries"
            }
          ]
        }
      }
    },
    {
      "id": "1032",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "abeillei",
        "species_class": "Aves",
        "sub_species": "Abeillia abeillei",
        "species_family": "Trochilidae",
        "species_kingdom": "Animalia",
        "scientific_name": "(Lesson & DeLattre, 1839)",
        "cites_status": "II",
        "cites_id": 3734,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": [
            {
              "id": "196",
              "type": "countries"
            },
            {
              "id": "170",
              "type": "countries"
            },
            {
              "id": "130",
              "type": "countries"
            },
            {
              "id": "124",
              "type": "countries"
            },
            {
              "id": "20",
              "type": "countries"
            }
          ]
        }
      }
    },
    {
      "id": "841",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "abelii",
        "species_class": "Mammalia",
        "sub_species": "Pongo abelii",
        "species_family": "Hominidae",
        "species_kingdom": "Animalia",
        "scientific_name": "Lesson, 1827",
        "cites_status": "I",
        "cites_id": 8203,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": [
            {
              "id": "30",
              "type": "countries"
            }
          ]
        }
      }
    },
    {
      "id": "9835",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "A.Berger",
        "species_class": "Liliaceae",
        "sub_species": "SPECIES",
        "species_family": "deserti",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Aloe spp.",
        "cites_id": 14717,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "8941",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "A.Berger",
        "species_class": "Euphorbiaceae",
        "sub_species": "SPECIES",
        "species_family": "franckiana",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Euphorbia spp.",
        "cites_id": 25357,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    }
  ],
  "links": {
    "first": "http://otp-staging.ipq.co/species?page%5Bnumber%5D=1",
    "prev": "http://otp-staging.ipq.co/species?page%5Bnumber%5D=1",
    "next": "http://otp-staging.ipq.co/species?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://otp-staging.ipq.co/species?page%5Bnumber%5D=2136&page%5Bsize%5D=10",
    "self": "http://otp-staging.ipq.co/species?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  },
  "meta": {
    "total_items": 21358
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the species of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/species?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (name, common_name, created_at, updated_at) | Text


> To obtain all species sorted by name:

```shell
curl -X GET http://localhost:3000/species?sort=name \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/species?sort=-name \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific species

To obtain specific species:

```shell
curl -X GET http://localhost:3000/species/33 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a Species

In order to create a species, you need an authorization token for current admin.

Only admin should be able to create Species

To create a species, you need to define all of the required fields in the request body. The fields that compose a species are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| name                | Name of the species                                           | Text    | Any Text                                       | Yes
| common_name         | Common Name of species                                        | Text    | Any Text                                       | No
| country_ids         | ID's of countries                                             | Array   | Valid countries ids array                      | No
| species_class       | Optional text                                                 | Text    | Any Text                                       | No
| sub_species         | Optional text                                                 | Text    | Any Text                                       | No
| sub_family          | Optional text                                                 | Text    | Any Text                                       | No
| sub_kingdom         | Optional text                                                 | Text    | Any Text                                       | No
| scientific_name     | Optional text                                                 | Text    | Any Text                                       | No
| cites_status        | Optional text                                                 | Text    | Any Text                                       | No
| cites_id            | Optional text                                                 | Number  | Any valid number                               | No
| iucn_status         | Optional text                                                 | Number  | Any valid number                               | No

> To create a species, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/species \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "species": {
      "name": "Species",
      "common_name": "Species",
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create species is an authenticated endpoint!
</aside>


## Updating a Species

In order to modify the species, you can PUT/PATCH a request.
It accepts the same parameters as the _create species_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/species/<species-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "species": {
      "name": "Another name for the species"
  }
}'
```

<aside class="notice">
Remember — create species is an authenticated endpoint!
</aside>

## Deleting a Species
You can delete a species! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/species/<species-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create species is an authenticated endpoint!
</aside>
