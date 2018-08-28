swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userid}/password:
    patch:
      summary: Resets user password by userid
      description: Resets user password by userid.
      operationId: resetPasswordById
      x-api-path-slug: usersuseridpassword-patch
      parameters:
      - in: body
        name: body
        description: New password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
      responses:
        200:
          description: OK
      tags:
      - Resets
      - User
      - Password
      - By
      - Userid
  /users/by-username/{username}/password:
    patch:
      summary: Resets user password by username
      description: Resets user password by username.
      operationId: resetPasswordByUsername
      x-api-path-slug: usersbyusernameusernamepassword-patch
      parameters:
      - in: body
        name: body
        description: New password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Resets
      - User
      - Password
      - By
      - Username