swagger: "2.0"
x-collection-name: Quovo
x-complete: 1
info:
  title: Quovo API v3
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me:
    put:
      summary: Update your password
      description: "Update your API password. All future requests to /v3/tokens must
        use the new password to properly authenticate.\r\n\r\nNew API passwords have
        several requirements:\r\n\r\n* Must be at least 6 characters long\r\n* Must
        contain a letter, a number, and a special character\r\n* Must not contain
        or be similar to your registered email or Quovo API username"
      operationId: MePut
      x-api-path-slug: me-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Your
      - Password