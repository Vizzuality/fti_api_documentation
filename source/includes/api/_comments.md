# Comments

Comments are available for annex operators, annex governances and observations

## Creating a comment

In order to create a comment, you need an authorization token.

Only admin, ngo or operator should be able to create comments

To create a comment, you need to define all of the required fields in the request body. The fields that compose a comment are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| commentable_type    | Type of commentable                                           | Text    | AnnexGovernance, AnnexOperator, Observation    | Yes
| commentable_id      | ID of commentable                                             | Integer | Valid ID                                       | Yes
| body                | Comment's text                                                | Text    | Any Text                                       | Yes

> To create a comment on annex_operator, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/annex_operators/<annex_operator-id>/comments \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "comment": {
      "commentable_type": "AnnexOperator",
      "commentable_id": 1,
      "body": "Lorem ipsum.."
  }
}'
```

> To create a comment on annex_government, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/annex_governments/<annex_government-id>/comments \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "comment": {
      "commentable_type": "AnnexGovernment",
      "commentable_id": 1,
      "body": "Lorem ipsum.."
  }
}'
```

> To create a comment on observation, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/observations/<observation-id>/comments \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "comment": {
      "commentable_type": "Observation",
      "commentable_id": 1,
      "body": "Lorem ipsum.."
  }
}'
```

<aside class="notice">
  Remember that create comment is an authenticated endpoint!
</aside>


## Deleting a Comment
You can delete a comment! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/annex_operators/<annex_operator-id>/comments/<comment-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create annex_operator is an authenticated endpoint!
</aside>
