---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 0
info:
  title: Auth0 Stats API Get Active Users
  version: v1
  description: Gets the active users count (logged in during the last 30 days).
host: login.auth0.com
basePath: /stats
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/stats/active-users:
    get:
      summary: Get Active Users
      description: Gets the active users count (logged in during the last 30 days).
      operationId: get_active-users
      x-api-path-slug: apiv2statsactiveusers-get
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Active
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