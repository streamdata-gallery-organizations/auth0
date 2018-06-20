---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 0
info:
  title: Auth0 Jobs API Jobs Job
  version: v1
  description: jobs job.
host: login.auth0.com
basePath: /jobs
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/jobs/users-imports:
    post:
      summary: Jobs Users Imports
      description: jobs users imports.
      operationId: post_users-imports
      x-api-path-slug: apiv2jobsusersimports-post
      parameters:
      - in: form
        name: connection_name
        description: The name of the connection to which users will be added
      - in: form
        name: users
        description: A file containing the users to import
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Users
      - Imports
  /api/v2/jobs/{job_id}:
    get:
      summary: Jobs Job
      description: jobs job.
      operationId: get_jobs_by_job_id
      x-api-path-slug: apiv2jobsjob-id-get
      parameters:
      - in: path
        name: job_id
        description: The id of the job
      responses:
        200:
          description: OK
      tags:
      - Jobs
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