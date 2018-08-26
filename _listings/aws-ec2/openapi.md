---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeKeyPairs:
    get:
      summary: Describe Key Pairs
      description: Describes one or more of your key pairs.
      operationId: describekeypairs
      x-api-path-slug: actiondescribekeypairs-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: KeyName
        description: A unique name for the key pair
        type: string
      - in: query
        name: PublicKeyMaterial
        description: The public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Paris
---