{
  "info": {
    "name": "Context.IO Get Discovery",
    "_postman_id": "2bd8a9ea-6811-403f-bbb7-dc03b6f11b6f",
    "description": "Attempts to discover IMAP settings for a given email address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "7b491511-3fbb-4445-b481-7cf88e13aed5",
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
              "id": "e364ddc9-e589-4501-b597-0af21c3f785a"
            }
          ]
        },
        {
          "id": "9ed716ac-8b9e-4c33-8d2d-b760a4b0d823",
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
              "id": "1fa1f93f-e25c-4d9e-9593-bad693262f39"
            }
          ]
        },
        {
          "id": "e48bbc44-bd8e-44ba-b7ae-05d42ffeab59",
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
              "id": "c3236486-c476-4baf-ad05-50fb536aabaf"
            }
          ]
        },
        {
          "id": "0f8d5d04-1922-4db7-8b93-0b1d73f30e91",
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
              "id": "15cd774e-d3b6-4f96-bfcc-f945c732b89b"
            }
          ]
        }
      ]
    },
    {
      "name": "Discovery",
      "item": [
        {
          "id": "4e7c8775-ca0f-482a-aae0-61b408c1ee9d",
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
              "id": "be2e6b75-8f4f-43a3-b4ee-4e3188e49ee5"
            }
          ]
        }
      ]
    }
  ]
}