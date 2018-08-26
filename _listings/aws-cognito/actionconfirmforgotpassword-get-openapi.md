---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Confirm Forgot Password
  version: 1.0.0
  description: |-
    Allows a user to enter a code provided when they reset their password to update
                their password.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ChangePassword:
    get:
      summary: Change Password
      description: Changes the password for a specified user in a user pool.
      operationId: changePassword
      x-api-path-slug: actionchangepassword-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token in the change password request
        type: string
      - in: query
        name: PreviousPassword
        description: The old password in the change password request
        type: string
      - in: query
        name: ProposedPassword
        description: The new password in the change password request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Password
  /?Action=AdminResetUserPassword:
    get:
      summary: Admin Reset User Password
      description: Resets the specified user's password in a user pool as an administrator.
      operationId: adminResetUserPassword
      x-api-path-slug: actionadminresetuserpassword-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user whose password you wish to reset
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to reset the
          users            password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Passwords
  /?Action=ConfirmForgotPassword:
    get:
      summary: Confirm Forgot Password
      description: |-
        Allows a user to enter a code provided when they reset their password to update
                    their password.
      operationId: confirmForgotPassword
      x-api-path-slug: actionconfirmforgotpassword-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: ConfirmationCode
        description: The confirmation code sent by a users request to retrieve a forgotten            password
        type: string
      - in: query
        name: Password
        description: The password sent by sent by a users request to retrieve a forgotten            password
        type: string
      - in: query
        name: SecretHash
        description: A keyed-hash message authentication code (HMAC) calculated using
          the secret key of            a user pool client and username plus the client
          ID in the message
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you want to enter a code to
          retrieve a forgotten            password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Passwords
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