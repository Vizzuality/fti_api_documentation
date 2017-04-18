# Species

## How obtain all species

To obtain all species:

```shell
curl -X GET http://localhost:3000/species \
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
      "id": "10353",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": " (G.Lodd.) Pridgeon & M.W.Chase",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "saurocephala",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 66888,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "10289",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(?Mast) emend. Danser",
        "species_class": "Nepenthaceae",
        "sub_species": "SPECIES",
        "species_family": "stenophylla",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Nepenthes spp.",
        "cites_id": 20618,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "16704",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(A. Rich & Gal.) L.O. Williams",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "grandiflora",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 14483,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "19956",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(A. Rich. & Galeotti) Balogh",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "chloraeformis",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 19331,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "19975",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(A. Rich. & Galeotti) Garay",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "violacea",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 19869,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "10948",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(A. Rich. & Galeotti) Garay",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "saccata",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 18073,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "18269",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(A. Rich. & Galeotti) Rolfe 1917",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "galeottiana",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 21990,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "14054",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(A. Rich. & Galeotti) Schltr.",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "mexicana",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 19354,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "16296",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(A. Rich. & Galeotti) Schltr.",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "sarcoglossa",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 20737,
        "iucn_status": null
      },
      "relationships": {
        "countries": {
          "data": []
        }
      }
    },
    {
      "id": "15826",
      "type": "species",
      "attributes": {
        "common_name": null,
        "name": "(A. Rich. & H.G.Galeotti) Dressler",
        "species_class": "Orchidaceae",
        "sub_species": "SPECIES",
        "species_family": "subulatifolia",
        "species_kingdom": "Plantae",
        "scientific_name": "II",
        "cites_status": "Orchidaceae spp.",
        "cites_id": 26292,
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
    "first": "http://localhost:3000/species?page%5Bnumber%5D=1",
    "prev": "http://localhost:3000/species?page%5Bnumber%5D=1",
    "next": "http://localhost:3000/species?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://localhost:3000/species?page%5Bnumber%5D=2136&page%5Bsize%5D=10",
    "self": "http://localhost:3000/species?page%5Bnumber%5D=1&page%5Bsize%5D=10"
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
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/species?sort=-name \
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific species

To obtain specific species:

```shell
curl -X GET http://localhost:3000/species/33 \
-H "OTP_API_KEY: Bearer <your-api-key>" \
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
-H "OTP_API_KEY: Bearer <your-api-key>" \
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
-H "OTP_API_KEY: Bearer <your-api-key>" \
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
-H "OTP_API_KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create species is an authenticated endpoint!
</aside>
