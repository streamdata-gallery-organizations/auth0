---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 0
info:
  title: Auth0 Users API Deletes a multifactor provider for a user.
  version: v1
  description: Deletes a multifactor provider for a user..
host: login.auth0.com
basePath: /users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/users/{id}/multifactor/{provider}:
    delete:
      summary: Deletes a multifactor provider for a user.
      description: Deletes a multifactor provider for a user..
      operationId: delete_multifactor_by_provider
      x-api-path-slug: apiv2usersidmultifactorprovider-delete
      parameters:
      - in: path
        name: id
        description: The user_id of the user to delete
      - in: path
        name: provider
        description: The multifactor provider
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Multifactor
      - Provider
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