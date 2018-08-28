---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Send password reset email
  description: |-
    Send an email containing a link for resetting the user's password. The link will contain a one-use, timed recovery code tied to the user's account. Only works for non-SSO users.
    ##### Permissions
    No permissions required.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/password/reset:
    post:
      summary: Reset password
      description: |-
        Update the password for a user using a one-use, timed recovery code tied to the user's account. Only works for non-SSO users.
        ##### Permissions
        No permissions required.
      operationId: update-the-password-for-a-user-using-a-oneuse-timed-recovery-code-tied-to-the-users-account-only-wor
      x-api-path-slug: userspasswordreset-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Password
  /users/{user_id}/password:
    put:
      summary: Update a user's password
      description: |-
        Update a user's password. New password must meet password policy set by server configuration. Current password is required if you're updating your own password.
        ##### Permissions
        Must be logged in as the user the password is being changed for or have `manage_system` permission.
      operationId: update-a-users-password-new-password-must-meet-password-policy-set-by-server-configuration-current-p
      x-api-path-slug: usersuser-idpassword-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Password
  /users/password/reset/send:
    post:
      summary: Send password reset email
      description: |-
        Send an email containing a link for resetting the user's password. The link will contain a one-use, timed recovery code tied to the user's account. Only works for non-SSO users.
        ##### Permissions
        No permissions required.
      operationId: send-an-email-containing-a-link-for-resetting-the-users-password-the-link-will-contain-a-oneuse-time
      x-api-path-slug: userspasswordresetsend-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Password
      - Reset
      - Email
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