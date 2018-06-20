---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 0
info:
  title: Auth0 API Get Clients
  version: 1.0.0
  description: Get clients.
host: login.auth0.com
basePath: /clients
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/clients:
    get:
      summary: Get Clients
      description: Get clients.
      operationId: get_clients
      x-api-path-slug: apiv2clients-get
      parameters:
      - in: query
        name: exclude_fields
        description: true if the fields specified are to be excluded from the result,
          false otherwise
      - in: query
        name: fields
        description: A comma separated list of fields to include or exclude (depending
          on exclude_fields) from the result
      responses:
        200:
          description: OK
      tags:
      - Clients
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