---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 0
info:
  title: Auth0 Stats API Get Daily Stats
  version: v1
  description: Gets the daily stats for a particular period.
host: login.auth0.com
basePath: /stats
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/stats/daily:
    get:
      summary: Get Daily Stats
      description: Gets the daily stats for a particular period.
      operationId: get_daily
      x-api-path-slug: apiv2statsdaily-get
      parameters:
      - in: query
        name: from
        description: The first day of the period (inclusive) in YYYYMMDD format
      - in: query
        name: to
        description: The last day of the period (inclusive) in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Daily
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