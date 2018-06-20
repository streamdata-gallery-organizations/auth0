{
  "info": {
    "name": "Auth0 Stats API Get Active Users",
    "_postman_id": "bbf83a83-3f95-4357-ac70-8fdb370ad821",
    "description": "Gets the active users count (logged in during the last 30 days).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stats",
      "item": [
        {
          "id": "7f221f47-dc87-416d-a015-b073beb2591c",
          "name": "get_active-users",
          "request": {
            "url": "http://login.auth0.com/stats/api/v2/stats/active-users",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the active users count (logged in during the last 30 days)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bea5c905-67f4-4856-90dc-3df85ba70d66"
            }
          ]
        }
      ]
    }
  ]
}