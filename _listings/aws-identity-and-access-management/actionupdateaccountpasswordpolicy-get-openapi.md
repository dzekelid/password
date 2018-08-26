---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Update Account Password Policy
  version: 1.0.0
  description: Updates the password policy settings for the AWS account.
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
      description: Changes the password of the IAM user who is calling this action.
      operationId: changePassword
      x-api-path-slug: actionchangepassword-get
      parameters:
      - in: query
        name: NewPassword
        description: The new password
        type: string
      - in: query
        name: OldPassword
        description: The IAM users current password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Passwords
  /?Action=DeleteAccountPasswordPolicy:
    get:
      summary: Delete Account Password Policy
      description: Deletes the password policy for the AWS account.
      operationId: deleteAccountPasswordPolicy
      x-api-path-slug: actiondeleteaccountpasswordpolicy-get
      parameters:
      - in: query
        name: LimitExceeded
        description: The request was rejected because it attempted to create resources
          beyond the current      AWS account limits
        type: string
      - in: query
        name: NoSuchEntity
        description: The request was rejected because it referenced an entity that
          does not exist
        type: string
      - in: query
        name: ServiceFailure
        description: The request processing has failed because of an unknown error,
          exception or      failure
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Password Policies
  /?Action=GetAccountPasswordPolicy:
    get:
      summary: Get Account Password Policy
      description: Retrieves the password policy for the AWS account.
      operationId: getAccountPasswordPolicy
      x-api-path-slug: actiongetaccountpasswordpolicy-get
      parameters:
      - in: query
        name: PasswordPolicy
        description: Contains information about the account password policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /?Action=UpdateAccountPasswordPolicy:
    get:
      summary: Update Account Password Policy
      description: Updates the password policy settings for the AWS account.
      operationId: updateAccountPasswordPolicy
      x-api-path-slug: actionupdateaccountpasswordpolicy-get
      parameters:
      - in: query
        name: AllowUsersToChangePassword
        description: Allows all IAM users in your account to use the AWS Management
          Console to change their own      passwords
        type: string
      - in: query
        name: HardExpiry
        description: Prevents IAM users from setting a new password after their password
          has      expired
        type: string
      - in: query
        name: MaxPasswordAge
        description: The number of days that an IAM user password is valid
        type: string
      - in: query
        name: MinimumPasswordLength
        description: The minimum number of characters allowed in an IAM user password
        type: string
      - in: query
        name: PasswordReusePrevention
        description: Specifies the number of previous passwords that IAM users are
          prevented from reusing
        type: string
      - in: query
        name: RequireLowercaseCharacters
        description: Specifies whether IAM user passwords must contain at least one
          lowercase character      from the ISO basic Latin alphabet (a to z)
        type: string
      - in: query
        name: RequireNumbers
        description: Specifies whether IAM user passwords must contain at least one
          numeric character (0      to 9)
        type: string
      - in: query
        name: RequireSymbols
        description: 'Specifies whether IAM user passwords must contain at least one
          of the following      non-alphanumeric characters:'
        type: string
      - in: query
        name: RequireUppercaseCharacters
        description: Specifies whether IAM user passwords must contain at least one
          uppercase character      from the ISO basic Latin alphabet (A to Z)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Password Policy
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