---
name: Rebilly
x-slug: rebilly
description: ""
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rebilly.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Password
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/password/master/_listings/rebilly/apis.md
specificationVersion: "0.14"
apis:
- name: Rebilly - Create a Reset Password Token
  x-api-slug: passwordtokens-post
  description: Create a Reset Password Token
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rebilly.png
  humanURL: https://www.rebilly.com
  baseURL: https://api.rebilly.com//v2.1
  tags: Billing, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/password/master/_listings/rebilly/passwordtokens-post-openapi.md
- name: Rebilly - Delete a Reset Password Token
  x-api-slug: passwordtokensid-delete
  description: Delete a Reset Password Token with predefined identifier string
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rebilly.png
  humanURL: https://www.rebilly.com
  baseURL: https://api.rebilly.com//v2.1
  tags: Billing, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/password/master/_listings/rebilly/passwordtokensid-delete-openapi.md
- name: Rebilly - Retrieve a Reset Password Token
  x-api-slug: passwordtokensid-get
  description: Retrieve a Reset Password Token with specified identifier string
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rebilly.png
  humanURL: https://www.rebilly.com
  baseURL: https://api.rebilly.com//v2.1
  tags: Billing, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/password/master/_listings/rebilly/passwordtokensid-get-openapi.md
- name: Rebilly - Sends an email with a link containing a token to reset user password
  x-api-slug: forgotpassword-post
  description: Sends an email with a link containing a token to reset user password
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rebilly.png
  humanURL: https://www.rebilly.com
  baseURL: https://api.rebilly.com//v2.1
  tags: Billing, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/password/master/_listings/rebilly/forgotpassword-post-openapi.md
- name: Rebilly - Create a session with email and password
  x-api-slug: signin-post
  description: Create a session with email and password
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rebilly.png
  humanURL: https://www.rebilly.com
  baseURL: https://api.rebilly.com//v2.1
  tags: Billing, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/password/master/_listings/rebilly/signin-post-openapi.md
- name: Rebilly - Reset user password
  x-api-slug: usersresetpasswordtoken-post
  description: Reset user password
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rebilly.png
  humanURL: https://www.rebilly.com
  baseURL: https://api.rebilly.com//v2.1
  tags: Billing, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/password/master/_listings/rebilly/usersresetpasswordtoken-post-openapi.md
- name: Rebilly - Updates user's password with the specified newPassword
  x-api-slug: usersidpassword-post
  description: Updates user's password with the specified newPassword. And checks
    if currentPassword matches the actual one.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rebilly.png
  humanURL: https://www.rebilly.com
  baseURL: https://api.rebilly.com//v2.1
  tags: Billing, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/password/master/_listings/rebilly/usersidpassword-post-openapi.md
x-common:
- type: x-website
  url: https://www.rebilly.com
- type: x-api-gallery
  url: http://rat.genome.database.api.gallery.streamdata.io
- type: x-api-stack
  url: http://rebilly.stack.network
- type: x-documentation
  url: https://rebilly.github.io/RebillyAPI/#
- type: x-github
  url: https://github.com/Rebilly
- type: x-license-agreement
  url: https://www.rebilly.com/api-license/
- type: x-openapi
  url: https://rebilly.github.io/RebillyAPI/swagger.json
- type: x-pricing
  url: https://www.rebilly.com/pricing/
- type: x-privacy-policy
  url: https://www.rebilly.com/privacy-policy/
- type: x-support
  url: https://help.rebilly.com/
- type: x-terms-of-service
  url: https://www.rebilly.com/terms-of-use/
- type: x-twitter
  url: https://twitter.com/RebillyInc
- type: x-website
  url: http://rebilly.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---