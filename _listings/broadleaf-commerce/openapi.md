---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customer/password:
    post:
      summary: Post Customer Password
      description: Post customer password.
      operationId: postCustomerPassword
      x-api-path-slug: customerpassword-post
      parameters:
      - in: body
        name: changePasswordForm
        description: changePasswordForm
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Password
---