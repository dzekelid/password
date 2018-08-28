---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Delete a Reset Password Token
  description: Delete a Reset Password Token with predefined identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /password-tokens:
    post:
      summary: Create a Reset Password Token
      description: Create a Reset Password Token
      operationId: password_tokens.post
      x-api-path-slug: passwordtokens-post
      parameters:
      - in: body
        name: body
        description: ResetPasswordToken resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Password
      - Token
  /password-tokens/{id}:
    delete:
      summary: Delete a Reset Password Token
      description: Delete a Reset Password Token with predefined identifier string
      operationId: password_tokens.id.delete
      x-api-path-slug: passwordtokensid-delete
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Password
      - Token
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