{
  "info": {
    "name": "Context.IO Post Oauth Provers",
    "_postman_id": "4c66db5d-6aff-40a7-b48b-7f7412bbb4da",
    "description": "Adds a new OAuth provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "ade45325-2979-4687-8527-2bda4c8de628",
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
              "id": "6e791262-0c86-4e8c-a8be-fd33e6052e96"
            }
          ]
        },
        {
          "id": "49d0f76c-d4c5-4ed7-a5a7-9aaab83ebf91",
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
              "id": "fec82036-edbb-4c8b-9194-31582b312630"
            }
          ]
        }
      ]
    }
  ]
}