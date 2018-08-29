{
  "info": {
    "name": "Auth0 Users API Gets all users who have logged in.",
    "_postman_id": "649df644-bdfa-4167-a670-1ebd68a899c2",
    "description": "Gets all users who have logged in..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "86911368-fb3d-4b80-9a98-fddde4c152cc",
          "name": "get_users",
          "request": {
            "url": "http://login.auth0.com/users/api/v2/users?connection=%7B%7D&exclude_fields=%7B%7D&fields=%7B%7D&include_totals=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all users who have logged in.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "758e211c-37fa-46e0-9b1b-0509a6969242"
            }
          ]
        },
        {
          "id": "7f37646e-d327-43e2-bf13-382826868c43",
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
              "id": "732a7d9a-87cb-44bb-91cd-81ec302d7109"
            }
          ]
        }
      ]
    }
  ]
}