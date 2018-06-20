---
swagger: "2.0"
x-collection-name: Auth0
x-complete: 0
info:
  title: Auth0 Users API Gets a user.
  version: v1
  description: Gets a user..
host: login.auth0.com
basePath: /users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v2/users:
    delete:
      summary: Deletes all users.
      description: Deletes all users. use with caution.
      operationId: delete_users
      x-api-path-slug: apiv2users-delete
      responses:
        200:
          description: OK
      tags:
      - Users
    get:
      summary: Gets all users who have logged in.
      description: Gets all users who have logged in..
      operationId: get_users
      x-api-path-slug: apiv2users-get
      parameters:
      - in: query
        name: connection
        description: Connection filter
      - in: query
        name: exclude_fields
        description: true if the fields specified are to be excluded from the result,
          false otherwise
      - in: query
        name: fields
        description: A comma separated list of fields to include or exclude (depending
          on exclude_fields) from the result
      - in: query
        name: include_totals
        description: true if a query summary must be included in the result
      - in: query
        name: page
        description: The page number
      - in: query
        name: per_page
        description: The amount of entries per page
      - in: query
        name: sort
        description: The field to use for sorting
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Creates a user.
      description: Creates a user..
      operationId: post_users
      x-api-path-slug: apiv2users-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
  /api/v2/users/{id}:
    delete:
      summary: Deletes a user.
      description: Deletes a user..
      operationId: delete_users_by_id
      x-api-path-slug: apiv2usersid-delete
      parameters:
      - in: path
        name: id
        description: The user_id of the user to delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
    get:
      summary: Gets a user.
      description: Gets a user..
      operationId: get_users_by_id
      x-api-path-slug: apiv2usersid-get
      parameters:
      - in: query
        name: exclude_fields
        description: true if the fields specified are to be excluded from the result,
          false otherwise
      - in: query
        name: fields
        description: A comma separated list of fields to include or exclude (depending
          on exclude_fields) from the result
      - in: path
        name: id
        description: The user_id of the user to retrieve
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
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