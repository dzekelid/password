swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
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
  /api/v1/password/forgot:
    post:
      summary: Post Password Forgot
      description: Post password forgot.
      operationId: postApiV1PasswordForgot
      x-api-path-slug: apiv1passwordforgot-post
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
      - Password
      - Forgot
  /api/v1/password/restore:
    post:
      summary: Post Password Restore
      description: Post password restore.
      operationId: postApiV1PasswordRestore
      x-api-path-slug: apiv1passwordrestore-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Password
      - Restore
  /api/v1/password/change:
    post:
      summary: Post Password Change
      description: Post password change.
      operationId: postApiV1PasswordChange
      x-api-path-slug: apiv1passwordchange-post
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
      - Password
      - Change