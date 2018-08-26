---
swagger: "2.0"
x-collection-name: Salesforce
x-complete: 1
info:
  title: Salesforce Sandbox
  description: create-sandbox-copies-of-your-environments-for-development-testing-and-training-without-compromising-the-data-and-applications-in-your-production-environment-
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
    delete:
      summary: Delete Version Sobjects User Password
      description: Resets an user password. Salesforce will reset the user password
        to an auto-generated password, which will be returned in the response.
      operationId: deleteVersionSobjectsUserPassword
      x-api-path-slug: versionsobjectsuseridpassword-delete
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
---