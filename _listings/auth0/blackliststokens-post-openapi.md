---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 0
info:
  title: Auth0 API Post Blacklists Tokens
  description: Post blacklists tokens.
  version: 1.0.0
host: login.auth0.com
basePath: api/v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blacklists/tokens:
    post:
      summary: Post Blacklists Tokens
      description: Post blacklists tokens.
      operationId: postBlacklistsTokens
      x-api-path-slug: blackliststokens-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blacklists
      - Tokens
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