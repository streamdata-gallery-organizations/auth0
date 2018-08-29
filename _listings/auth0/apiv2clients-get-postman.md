{
  "info": {
    "name": "Auth0 API Get Clients",
    "_postman_id": "e7bbdff7-8274-4952-b6ae-98036c1a8bb7",
    "description": "Get clients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clients",
      "item": [
        {
          "id": "141635f4-0c9b-4bff-9d00-5605ab50d4d3",
          "name": "get_clients",
          "request": {
            "url": "http://login.auth0.com/clients/api/v2/clients?exclude_fields=%7B%7D&fields=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get clients."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "643053d2-f821-46f1-b0dd-8972fe91e721"
            }
          ]
        }
      ]
    }
  ]
}