{
  "info": {
    "name": "Context.IO Post Connect Tokens",
    "_postman_id": "627f7ec4-b621-442e-9c52-ad8430666f3c",
    "description": "Obtains a new connect_token.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "d1053a21-f5fa-47f2-a5c7-81b6c51f06a6",
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
              "id": "3b49ec21-06d1-4134-9898-8f59fd24109d"
            }
          ]
        },
        {
          "id": "a8bee6eb-16d9-4cb4-9061-97645216e176",
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
              "id": "1ae73e5d-a9e5-474c-a1ec-1aac43f3b6e1"
            }
          ]
        },
        {
          "id": "e6034b3f-56e3-4174-a715-4e93cfe7b577",
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
              "id": "a9323861-0863-40c5-b9ec-84961e836e13"
            }
          ]
        },
        {
          "id": "3608cd5f-e5b5-45ee-abbf-e9cc637abf0e",
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
              "id": "5871fa07-f6d3-473d-b88a-eabb609f1a4b"
            }
          ]
        }
      ]
    },
    {
      "name": "Discovery",
      "item": [
        {
          "id": "462f94ef-6751-448b-bb7e-0bab5545705f",
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
              "id": "92b43945-83ba-4d92-b832-55f48838dcc0"
            }
          ]
        }
      ]
    },
    {
      "name": "Connect",
      "item": [
        {
          "id": "2f677325-5313-4b85-8b19-f31fabc45c9e",
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
              "id": "fd2b36a0-42ed-4789-82d7-e8e55f235a98"
            }
          ]
        },
        {
          "id": "dc4f0813-5c9e-43d0-b652-3b0d94e5206a",
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
              "id": "36818e0e-46f4-43a8-8f98-c66adbcce54a"
            }
          ]
        }
      ]
    }
  ]
}