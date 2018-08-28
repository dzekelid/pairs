---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Get Key Pairs
  version: 1.0.0
  description: Returns information about all key pairs in the user's account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetKeyPairs:
    get:
      summary: Get Key Pairs
      description: Returns information about all key pairs in the user's account.
      operationId: getKeyPairs
      x-api-path-slug: actiongetkeypairs-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get key pairs      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---