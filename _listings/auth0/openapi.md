swagger: "2.0"
x-collection-name: Auth0
x-complete: 1
info:
  title: Auth0 Users API
  version: v1
host: login.auth0.com
basePath: /users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blacklists/tokens:
    get:
      summary: Get Blacklists Tokens
      description: Get blacklists tokens.
      operationId: getBlacklistsTokens
      x-api-path-slug: blackliststokens-get
      parameters:
      - in: query
        name: aud
        description: The JWTs aud claim
      responses:
        200:
          description: OK
      tags:
      - Blacklists
      - Tokens
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
  /clients:
    get:
      summary: Get Clients
      description: Get clients.
      operationId: getClients
      x-api-path-slug: clients-get
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
    post:
      summary: Post Clients
      description: Post clients.
      operationId: postClients
      x-api-path-slug: clients-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clients
  /clients/{id}:
    delete:
      summary: Delete Clients
      description: Delete clients.
      operationId: deleteClients
      x-api-path-slug: clientsid-delete
      parameters:
      - in: path
        name: id
        description: The client_id of the client to delete
      responses:
        200:
          description: OK
      tags:
      - Clients
    get:
      summary: Get Clients
      description: Get clients.
      operationId: getClients
      x-api-path-slug: clientsid-get
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
        description: The client_id of the client to retrieve
      responses:
        200:
          description: OK
      tags:
      - Clients
    patch:
      summary: Patch Clients
      description: Patch clients.
      operationId: patchClients
      x-api-path-slug: clientsid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The client_id of the client to retrieve
      responses:
        200:
          description: OK
      tags:
      - Clients
  /jobs/users-imports:
    post:
      summary: Post Jobs Users Imports
      description: Post jobs users imports.
      operationId: postJobsUsersImports
      x-api-path-slug: jobsusersimports-post
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
      - Immports
  /jobs/{job_id}:
    get:
      summary: Get Jobs Job
      description: Get jobs job.
      operationId: getJobsJob
      x-api-path-slug: jobsjob-id-get
      parameters:
      - in: path
        name: job_id
        description: The id of the job
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /stats/active-users:
    get:
      summary: Get Stats Active Users
      description: Get stats active users.
      operationId: getStatsActiveUsers
      x-api-path-slug: statsactiveusers-get
      responses:
        200:
          description: OK
      tags:
      - Statistics
  /stats/daily:
    get:
      summary: Get Stats Daily
      description: Get stats daily.
      operationId: getStatsDaily
      x-api-path-slug: statsdaily-get
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
      - Statistics
      - Daily
  /users:
    delete:
      summary: Delete Users
      description: Delete users.
      operationId: deleteUsers
      x-api-path-slug: users-delete
      responses:
        200:
          description: OK
      tags:
      - Users
    get:
      summary: Get Users
      description: Get users.
      operationId: getUsers
      x-api-path-slug: users-get
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
      summary: Post Users
      description: Post users.
      operationId: postUsers
      x-api-path-slug: users-post
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
  /users/{id}:
    delete:
      summary: Delete Users
      description: Delete users.
      operationId: deleteUsers
      x-api-path-slug: usersid-delete
      parameters:
      - in: path
        name: id
        description: The user_id of the user to delete
      responses:
        200:
          description: OK
      tags:
      - Users
    get:
      summary: Get Users
      description: Get users.
      operationId: getUsers
      x-api-path-slug: usersid-get
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
    patch:
      summary: Patch Users
      description: Patch users.
      operationId: patchUsers
      x-api-path-slug: usersid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The user_id of the user to update
      responses:
        200:
          description: OK
      tags:
      - Users
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
  /api/v2/blacklists/tokens:
    get:
      summary: Get Blacklists Tokens
      description: Get blacklists tokens.
      operationId: get_tokens
      x-api-path-slug: apiv2blackliststokens-get
      parameters:
      - in: query
        name: aud
        description: The JWTs aud claim
      responses:
        200:
          description: OK
      tags:
      - Blacklists
      - Tokens
    post:
      summary: Post Blacklists Tokens
      description: Post blacklists tokens.
      operationId: post_tokens
      x-api-path-slug: apiv2blackliststokens-post
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
    patch:
      summary: Updates a user.
      description: Updates a user..
      operationId: patch_users_by_id
      x-api-path-slug: apiv2usersid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The user_id of the user to update
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
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