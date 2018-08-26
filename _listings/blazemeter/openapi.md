---
swagger: "2.0"
x-collection-name: BlazeMeter
x-complete: 1
info:
  title: Blazemeter API Explorer
  description: live-api-documentation
  version: 1.0.0
host: a.blazemeter.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/password:
    patch:
      summary: Patch User Password
      description: Patch user password.
      operationId: user.password.patch
      x-api-path-slug: userpassword-patch
      parameters:
      - in: body
        name: blazemeter\Routing\v4\UserModel1
        description: currentPassword (required)newPassword (required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Password
    post:
      summary: Post User Password
      description: Post user password.
      operationId: user.password.post
      x-api-path-slug: userpassword-post
      parameters:
      - in: body
        name: blazemeter\Routing\v4\UserModel3
        description: currentPassword (required)newPassword (required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Password
    put:
      summary: Put User Password
      description: Put user password.
      operationId: user.password.put
      x-api-path-slug: userpassword-put
      parameters:
      - in: body
        name: blazemeter\Routing\v4\UserModel2
        description: currentPassword (required)newPassword (required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Password
---