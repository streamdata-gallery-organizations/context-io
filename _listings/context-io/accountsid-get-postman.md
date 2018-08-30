{
  "info": {
    "name": "Context.IO Get Accounts",
    "_postman_id": "0344d6ce-8917-4d78-8208-fb6791d765ca",
    "description": "Gets details about a given account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "98127621-5314-4641-a5b4-b344ba34f6d7",
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
              "id": "39f85016-914e-4ee6-9642-1297c89377a7"
            }
          ]
        },
        {
          "id": "7adfead6-e859-4274-9d87-bcae5942067c",
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
              "id": "b51eefaf-fcaa-4c3f-b5bc-df1e49087450"
            }
          ]
        },
        {
          "id": "d65b03bf-b9f5-4c45-b4b2-6881ba106851",
          "name": "getAccount_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details about a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9681f8f0-aa9d-40bd-a3a8-d28488d5976d"
            }
          ]
        }
      ]
    }
  ]
}