---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 0
info:
  title: Quovo Update your password
  description: "Update your API password. All future requests to /v3/tokens must use
    the new password to properly authenticate.\r\n\r\nNew API passwords have several
    requirements:\r\n\r\n* Must be at least 6 characters long\r\n* Must contain a
    letter, a number, and a special character\r\n* Must not contain or be similar
    to your registered email or Quovo API username"
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