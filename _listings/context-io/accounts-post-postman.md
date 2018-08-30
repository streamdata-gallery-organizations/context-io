{
  "info": {
    "name": "Context.IO Post Accounts",
    "_postman_id": "ca10d11a-e358-4421-b76b-8279dd8e4d88",
    "description": "Adds a new account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "f2b672de-29e7-4aa5-bf64-3fc8fd98d96f",
          "name": "listAccounts_",
          "request": {
            "url": "http://api.context.io/2.0/accounts?email=%7B%7D&limit=%7B%7D&offset=%7B%7D&status=%7B%7D&status_ok=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "984a1f2d-f7e8-4a4c-9cee-b680810cec29"
            }
          ]
        },
        {
          "id": "ba564f27-931a-4f0d-9069-662ff6f7ff42",
          "name": "addAccount_",
          "request": {
            "url": "http://api.context.io/2.0/accounts?email=%7B%7D&first_name=%7B%7D&last_name=%7B%7D&token=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "988bdfc3-eb5e-4fbd-9ede-0fb8893b6b77"
            }
          ]
        }
      ]
    }
  ]
}