---
swagger: "2.0"
x-collection-name: Salesforce
x-complete: 0
info:
  title: Salesforce Sandbox Post Version Sobjects User Password
  description: Changes the password for a given user ID. The new password must conform
    to the password policies for the organization, otherwise you will get an error
    response. You can only change one password per request.
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/sobjects/User/{id}/password:
    get:
      summary: Get Version Sobjects User Password
      description: Gets password expiration status for a given user. The session must
        have permission to access the given user password information, otherwise an
        error response is returned.
      operationId: getVersionSobjectsUserPassword
      x-api-path-slug: versionsobjectsuseridpassword-get
      parameters:
      - in: path
        name: id
        description: A Salesforces user ID
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - User
      - Password
    post:
      summary: Post Version Sobjects User Password
      description: Changes the password for a given user ID. The new password must
        conform to the password policies for the organization, otherwise you will
        get an error response. You can only change one password per request.
      operationId: postVersionSobjectsUserPassword
      x-api-path-slug: versionsobjectsuseridpassword-post
      parameters:
      - in: path
        name: id
        description: A Salesforces user ID
      - in: path
        name: version
        description: An API version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Sobjects
      - User
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