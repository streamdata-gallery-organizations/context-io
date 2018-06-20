{
  "info": {
    "name": "Context.IO Delete Connect Tokens Token",
    "_postman_id": "14e8e753-c67c-4f76-bbe9-3b1675de4276",
    "description": "Removes a given connect token.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "7bc9e483-dfc5-44f3-b5ec-0835f607a789",
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
              "id": "91fc265e-660d-47ae-9363-a8fc446398f0"
            }
          ]
        },
        {
          "id": "f6739527-2de5-4a2e-9852-145aed6bffe0",
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
              "id": "da549330-fdfa-4a4a-b823-abc4542cbeab"
            }
          ]
        },
        {
          "id": "3f6dfe09-5da2-4791-b35b-4a0bb57f870c",
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
              "id": "8591950a-64c4-45d5-8484-56393fa40176"
            }
          ]
        },
        {
          "id": "819fe013-f9ef-49c9-b0e2-a7682c7d0fe4",
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
              "id": "f5b67d0b-c533-4d73-99ab-683cd43aca28"
            }
          ]
        }
      ]
    },
    {
      "name": "Discovery",
      "item": [
        {
          "id": "87fc001b-7ff2-4e39-8de9-e635a8d3224c",
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
              "id": "73900aeb-e858-45aa-babc-2b643ee1d0d6"
            }
          ]
        }
      ]
    },
    {
      "name": "Connect",
      "item": [
        {
          "id": "e182b2e7-f364-4580-a729-9bed6cd144f2",
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
              "id": "cfa03180-ce7d-4d09-abfb-5f60d39f02f9"
            }
          ]
        },
        {
          "id": "7e8ebcdb-90ca-4b95-aa19-490b57b116e5",
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
              "id": "0853c8e3-386e-4a07-9c23-ea3e9712249a"
            }
          ]
        },
        {
          "id": "3c0d91d9-d744-4e17-9a0f-fad8a5c9381b",
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
              "id": "b5cd338d-cd98-43c7-bc66-e6ff379857fe"
            }
          ]
        },
        {
          "id": "93a05554-c430-4b4e-a4bb-7cc8241fdda3",
          "name": "removeConnectToken_",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a given connect token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62c49334-1cd3-4285-a514-d2f91b6950de"
            }
          ]
        }
      ]
    }
  ]
}