{
  "info": {
    "name": "Context.IO Delete Oauth Provers Key",
    "_postman_id": "2266d47f-3866-4855-8f4e-835de9d570f3",
    "description": "Removes a given OAuth provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "e9591599-b2bf-4d43-a8d2-9034330b60e1",
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
              "id": "54f1008f-9613-4dd0-b7d9-fa0d0eb342ca"
            }
          ]
        },
        {
          "id": "db6ba7a7-0650-4966-8d61-cb498439dee4",
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
              "id": "af443028-9239-4bf0-8e82-7a36be6e54cb"
            }
          ]
        },
        {
          "id": "285e7522-058b-43ba-86c8-e44b7e74d1f3",
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
              "id": "e78760b6-fafe-47fd-b8bd-daff428f5053"
            }
          ]
        },
        {
          "id": "55028529-f2b9-4ada-b1e4-812b5dbf2ba2",
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
              "id": "750b716a-112b-4acd-95fc-e123b6fae227"
            }
          ]
        }
      ]
    }
  ]
}