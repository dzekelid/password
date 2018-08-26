---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/ChangePinAndPassword:
    post:
      summary: Add API Changepinandpassword
      description: Add api changepinandpassword.
      operationId: ApiChangePinAndPasswordPost
      x-api-path-slug: apichangepinandpassword-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Changepinandpassword
  /api/RemindPasswordEmail:
    post:
      summary: Add API Remindpasswordemail
      description: Add api remindpasswordemail.
      operationId: ApiRemindPasswordEmailPost
      x-api-path-slug: apiremindpasswordemail-post
      parameters:
      - in: body
        name: reqModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Remindpasswordemail
---