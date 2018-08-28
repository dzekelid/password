---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Updates user's password with the specified newPassword
  description: Updates user's password with the specified newPassword. And checks
    if currentPassword matches the actual one.
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
    get:
      summary: Retrieve a Reset Password Token
      description: Retrieve a Reset Password Token with specified identifier string
      operationId: password_tokens.id.get
      x-api-path-slug: passwordtokensid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Reset
      - Password
      - Token
  /forgot-password:
    post:
      summary: Sends an email with a link containing a token to reset user password
      description: Sends an email with a link containing a token to reset user password
      operationId: sends-an-email-with-a-link-containing-a-token-to-reset-user-password
      x-api-path-slug: forgotpassword-post
      parameters:
      - in: body
        name: body
        description: Email resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Email
      - Link
      - Containing
      - Token
      - To
      - Reset
      - User
      - Password
  /signin:
    post:
      summary: Create a session with email and password
      description: Create a session with email and password
      operationId: create-a-session-with-email-and-password
      x-api-path-slug: signin-post
      parameters:
      - in: body
        name: body
        description: Signin resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Session
      - Email
      - Password
  /users/reset-password/{token}:
    post:
      summary: Reset user password
      description: Reset user password
      operationId: reset-user-password
      x-api-path-slug: usersresetpasswordtoken-post
      parameters:
      - in: body
        name: body
        description: ResetPassword resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reset
      - User
      - Password
  /users/{id}/password:
    post:
      summary: Updates user's password with the specified newPassword
      description: Updates user's password with the specified newPassword. And checks
        if currentPassword matches the actual one.
      operationId: updates-users-password-with-the-specified-newpassword--and-checks-if-currentpassword-matches-the-act
      x-api-path-slug: usersidpassword-post
      parameters:
      - in: body
        name: body
        description: currentPassword and newPassword
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Users
      - Password
      - Specified
      - NewPassword
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