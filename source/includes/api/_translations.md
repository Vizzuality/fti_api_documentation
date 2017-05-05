# Translations

The OPEN TIMBER PORTAL API uses param locale to obtain and translate specific fields.

Available languages: (:en, :fr)

## Entities included in translations

| Entity          | Translated fields
| -------------   |:-------------:| -----:|
| AnnexGovernance | governance_pillar, governance_problem, details

## To translate specific entity

> An example update request for locale :fr:

```shell
curl -X PATCH http://localhost:3000/countries/<country-id>?locale=fr \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "country": {
      "name": "FR name for the country"
  }
}'
```
