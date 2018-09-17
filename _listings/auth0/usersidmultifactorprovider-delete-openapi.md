---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 0
info:
  title: Auth0 API Delete Users Multifactor Prover
  description: Delete users multifactor prover.
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
  /users/{id}/multifactor/{provider}:
    delete:
      summary: Delete Users Multifactor Prover
      description: Delete users multifactor prover.
      operationId: deleteUsersMultifactorProver
      x-api-path-slug: usersidmultifactorprovider-delete
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