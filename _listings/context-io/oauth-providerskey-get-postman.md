{
  "info": {
    "name": "Context.IO Get Oauth Provers Key",
    "_postman_id": "1fd275ff-677d-4065-b2ac-778cac9c7445",
    "description": "Gets information about a given OAuth provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "ccea198b-c61e-4157-91a3-6435b1366cf0",
          "name": "listOauthProviders_",
          "request": {
            "url": "http://api.context.io/2.0/oauth_providers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List configured OAuth providers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90e0b2ce-8bd6-43a6-95c5-0b29fcec6b52"
            }
          ]
        },
        {
          "id": "3c0912bb-8d34-4de8-b573-f26170751ac3",
          "name": "addOauthProviders_",
          "request": {
            "url": "http://api.context.io/2.0/oauth_providers?provider_consumer_key=%7B%7D&provider_consumer_secret=%7B%7D&type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new OAuth provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2741bb98-532b-470f-877b-b634c38a8937"
            }
          ]
        },
        {
          "id": "9341625e-23a0-431a-bde4-0d6f21d1e4b3",
          "name": "getOauthProvider_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "oauth_providers/:key"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a given OAuth provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2770ea30-0980-4c25-9164-07b859ae518a"
            }
          ]
        }
      ]
    }
  ]
}