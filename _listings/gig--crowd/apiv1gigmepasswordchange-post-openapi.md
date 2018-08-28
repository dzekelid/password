---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Gigme Password Change
  version: 1.0.0
  description: Post gigme password change.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/gigme/password/forgot:
    post:
      summary: Post Gigme Password Forgot
      description: Post gigme password forgot.
      operationId: postApiV1GigmePasswordForgot
      x-api-path-slug: apiv1gigmepasswordforgot-post
      parameters:
      - in: body
        name: request
        description: Email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Password
      - Forgot
  /api/v1/gigme/password/restore:
    post:
      summary: Post Gigme Password Restore
      description: Post gigme password restore.
      operationId: postApiV1GigmePasswordRestore
      x-api-path-slug: apiv1gigmepasswordrestore-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Password
      - Restore
  /api/v1/gigme/password/change:
    post:
      summary: Post Gigme Password Change
      description: Post gigme password change.
      operationId: postApiV1GigmePasswordChange
      x-api-path-slug: apiv1gigmepasswordchange-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Password
      - Change
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