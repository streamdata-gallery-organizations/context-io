{
  "info": {
    "name": "Context.IO Get Oauth Provers",
    "_postman_id": "8140ee54-20e0-447c-bb6f-f21cc519944d",
    "description": "List configured OAuth providers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Oauth",
      "item": [
        {
          "id": "9d3ba454-6459-49cf-b0f0-e1c749cbc0db",
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
              "id": "af619185-32ca-41a9-80ff-943c82f89fe1"
            }
          ]
        }
      ]
    }
  ]
}