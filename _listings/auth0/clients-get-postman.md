{
  "info": {
    "name": "Auth0 API Get Clients",
    "_postman_id": "97a07475-081f-40e1-a00d-f1040b02c4ef",
    "description": "Get clients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clients",
      "item": [
        {
          "id": "5cd23365-8e74-425d-9647-65cf841a6a57",
          "name": "getClients",
          "request": {
            "url": "http://login.auth0.com/api/v2/clients?exclude_fields=%7B%7D&fields=%7B%7D",
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
              "id": "07dcb189-6232-4e1f-a4ee-749fda8a86ae"
            }
          ]
        }
      ]
    }
  ]
}