{
  "info": {
    "name": "Context.IO Get Accounts",
    "_postman_id": "d7bfce6c-c54b-4fae-b233-b46df0ff0208",
    "description": "Lists accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "e3073f30-bc73-4487-99a9-82b8d145adf0",
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
              "id": "f3f3dc0e-3246-4778-8f18-91beef362c8a"
            }
          ]
        }
      ]
    }
  ]
}