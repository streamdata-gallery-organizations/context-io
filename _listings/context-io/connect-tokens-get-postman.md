{
  "info": {
    "name": "Context.IO Get Connect Tokens",
    "_postman_id": "4941160a-fc98-4cd4-94dc-5b2bc07bda9a",
    "description": "Lists connect tokens created with your API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "4666cbdd-a1cc-40ce-b764-8aef6a94cb5d",
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
              "id": "2029ee2c-fe1c-40ef-8f2e-92311df7e99e"
            }
          ]
        },
        {
          "id": "38df328c-7af7-4ce4-b089-3d699f2b01ba",
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
              "id": "e38d71b8-cf05-4533-86bf-9d4bb2501731"
            }
          ]
        },
        {
          "id": "b227a707-8a27-47b6-8869-93c1d0838ae9",
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
              "id": "6a5b96e7-7d17-4e13-9755-0c8be9b7b312"
            }
          ]
        },
        {
          "id": "4257697e-f090-467c-bb93-557afb9d4c80",
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
              "id": "97328eeb-d1f9-47a9-8f16-c90cae7980db"
            }
          ]
        }
      ]
    },
    {
      "name": "Discovery",
      "item": [
        {
          "id": "039a4a09-b058-4d42-a288-01b6c76baaab",
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
              "id": "2210cf01-47be-43f1-be34-19375b5822ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Connect",
      "item": [
        {
          "id": "65135435-8d0e-4684-b0bf-78bb896171d9",
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
              "id": "342b9aa7-ee3d-4795-b91d-a578a5606a34"
            }
          ]
        }
      ]
    }
  ]
}