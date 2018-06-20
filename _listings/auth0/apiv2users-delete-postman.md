{
  "info": {
    "name": "Auth0 Users API Deletes all users.",
    "_postman_id": "c05dfc34-6c23-4746-984b-19d23c63f08e",
    "description": "Deletes all users. use with caution.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "64498a31-4de3-4ece-8c0c-d7d8d6acb1f0",
          "name": "delete_users",
          "request": {
            "url": "http://login.auth0.com/users/api/v2/users",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes all users. use with caution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef80cc8a-1fcd-4e7b-919f-e50f93cb0114"
            }
          ]
        }
      ]
    }
  ]
}