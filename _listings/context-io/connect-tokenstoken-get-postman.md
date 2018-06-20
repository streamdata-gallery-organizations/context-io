{
  "info": {
    "name": "Context.IO Get Connect Tokens Token",
    "_postman_id": "2dcc3514-fd9f-405a-86fa-6b38e1fe3011",
    "description": "Gets information about a given connect token.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "b65aa47e-da1b-438a-be6d-eee2f376831f",
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
              "id": "02dd70e8-1c0d-40b6-be02-6e8587581016"
            }
          ]
        },
        {
          "id": "37a1a3b0-ad6c-480e-a68e-871f940182df",
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
              "id": "da23f77a-ddfb-4722-a88e-a765ccb97bdb"
            }
          ]
        },
        {
          "id": "ef5aab07-ab51-49cf-89c2-4fc90f8177d8",
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
              "id": "509b028d-dcdf-49cb-9020-b7a09c34b632"
            }
          ]
        },
        {
          "id": "80ab761f-ca76-4f99-93f6-ae4a029c1d5a",
          "name": "removeOauthProvider_",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a given OAuth provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19502352-e4e2-4182-b71f-6cd2ff728dcb"
            }
          ]
        }
      ]
    },
    {
      "name": "Discovery",
      "item": [
        {
          "id": "043d0007-897a-41ed-96ac-9b2708d5419d",
          "name": "Get_discoverEmailImapSettings_",
          "request": {
            "url": "http://api.context.io/2.0/discovery?email=%7B%7D&source_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to discover IMAP settings for a given email address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d123c41-1007-42cd-a6dd-d89a17593247"
            }
          ]
        }
      ]
    },
    {
      "name": "Connect",
      "item": [
        {
          "id": "814d00bb-78e6-4b9f-8bd5-56f45a9eecfe",
          "name": "listConnectTokens_",
          "request": {
            "url": "http://api.context.io/2.0/connect_tokens",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists connect tokens created with your API key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a3b9e56-61dd-4701-83c0-4093be4baf69"
            }
          ]
        },
        {
          "id": "ab42b873-abed-4fa6-81ac-f43a273ccd49",
          "name": "Create_obtainNewConnectToken_",
          "request": {
            "url": "http://api.context.io/2.0/connect_tokens?callback_url=%7B%7D&email=%7B%7D&first_name=%7B%7D&last_name=%7B%7D&service_level=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains a new connect_token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15a93c9c-e82a-405e-9f73-5511a9cf0ec7"
            }
          ]
        },
        {
          "id": "5f4a052b-b5c0-4b8d-98a4-8a9d5dbe0091",
          "name": "getConnectToken_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "connect_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a given connect token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e41a462-f39a-46fa-af85-5e2aa519ef6f"
            }
          ]
        }
      ]
    }
  ]
}