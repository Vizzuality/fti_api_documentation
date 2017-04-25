# Countries

## How obtain all countries

To obtain all countries:

```shell
curl -X GET http://localhost:3000/countries \
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
      "id": "220",
      "type": "countries",
      "attributes": {
        "iso": "AFG",
        "region_iso": "SC",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            33,
            66
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            35.3805743715067,
            68.9353807947497
          ]
        },
        "is_active": false,
        "name": "Afghanistan",
        "region_name": "South-Central Asia"
      }
    },
    {
      "id": "157",
      "type": "countries",
      "attributes": {
        "iso": "ALB",
        "region_iso": "SE",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            41,
            20
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            41.4578362811151,
            7.38956543946488
          ]
        },
        "is_active": false,
        "name": "Albania",
        "region_name": "Southern Europe"
      }
    },
    {
      "id": "221",
      "type": "countries",
      "attributes": {
        "iso": "DZA",
        "region_iso": "NA",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            28,
            3
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            25.1323592342349,
            14.8790854842834
          ]
        },
        "is_active": false,
        "name": "Algeria",
        "region_name": "North Africa"
      }
    },
    {
      "id": "122",
      "type": "countries",
      "attributes": {
        "iso": "ASM",
        "region_iso": "PO",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            -14.23377,
            -169.47767
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            -15.5658471700352,
            -165.562775258219
          ]
        },
        "is_active": false,
        "name": "American Samoa",
        "region_name": "Polynesia"
      }
    },
    {
      "id": "123",
      "type": "countries",
      "attributes": {
        "iso": "AND",
        "region_iso": "WE",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            42.55,
            1.58333
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            48.573968061361,
            6.45768472125939
          ]
        },
        "is_active": false,
        "name": "Andorra",
        "region_name": "Western Europe"
      }
    },
    {
      "id": "124",
      "type": "countries",
      "attributes": {
        "iso": "AGO",
        "region_iso": "MA",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            -12.5,
            18.5
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            0.618107263658459,
            19.464922564119
          ]
        },
        "is_active": false,
        "name": "Angola",
        "region_name": "Middle Africa"
      }
    },
    {
      "id": "125",
      "type": "countries",
      "attributes": {
        "iso": "AIA",
        "region_iso": "CB",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            18.21667,
            -63.05
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            20.2298014225409,
            -75.0918978909751
          ]
        },
        "is_active": false,
        "name": "Anguilla",
        "region_name": "Carribbean"
      }
    },
    {
      "id": "222",
      "type": "countries",
      "attributes": {
        "iso": "ATA",
        "region_iso": "AN",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            -82.67628,
            8.78906
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            -80.5079464102288,
            19.9088475268188
          ]
        },
        "is_active": false,
        "name": "Antarctica",
        "region_name": "Antartica"
      }
    },
    {
      "id": "223",
      "type": "countries",
      "attributes": {
        "iso": "ATG",
        "region_iso": "CB",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            17.05,
            -61.8
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            20.2298014225409,
            -75.0918978909751
          ]
        },
        "is_active": false,
        "name": "Antigua and Barbuda",
        "region_name": "Carribbean"
      }
    },
    {
      "id": "84",
      "type": "countries",
      "attributes": {
        "iso": "ARG",
        "region_iso": "SM",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            -34,
            -64
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            -15.2231547189536,
            -60.8171054886641
          ]
        },
        "is_active": false,
        "name": "Argentina",
        "region_name": "South America"
      }
    }
  ],
  "links": {
    "first": "http://localhost:3000/countries?page%5Bnumber%5D=1",
    "prev": "http://localhost:3000/countries?page%5Bnumber%5D=1",
    "next": "http://localhost:3000/countries?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://localhost:3000/countries?page%5Bnumber%5D=24&page%5Bsize%5D=10",
    "self": "http://localhost:3000/countries?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the countries of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/countries?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (name, created_at, updated_at) | Text


> To obtain all countries sorted by name:

```shell
curl -X GET http://localhost:3000/countries?sort=name \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/countries?sort=-name \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific country

To obtain specific country:

```shell
curl -X GET http://localhost:3000/countries/33 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a Country

In order to create a country, you need an authorization token for current admin.

Only admin should be able to create Countries

To create a country, you need to define all of the required fields in the request body. The fields that compose a country are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| name                | Name of the country                                           | Text   | Any Text                                        | Yes
| region_name         | Name of global region                                         | Text   | Any Text                                        | No
| region_centroid     | JSON data for centroid                                        | JSONB  | ANY JSON                                        | No
| country_centroid    | JSON data for centroid                                        | JSONB  | Any JSON                                        | No
| region_iso          | Ico of global region                                          | Text   | Valid region iso                                | No
| iso                 | Iso of the country                                            | Text   | Valid iso (ESP)                                 | Yes
| is_active           | Activate deactiveta countries (only accessible by admin)      | Boolean  | default value true                    | No


> To create a country, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/countries \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "country": {
      "name": "Spain",
      "iso": "ESP",
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create country is an authenticated endpoint!
</aside>


## Updating a Country

In order to modify the country, you can PUT/PATCH a request.
It accepts the same parameters as the _create country_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/countries/<country-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "country": {
      "name": "Another name for the country",
      "is_active": true
  }
}'
```

<aside class="notice">
Remember — create country is an authenticated endpoint!
</aside>

## Deleting a Country
You can delete a country! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/countries/<country-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create country is an authenticated endpoint!
</aside>
