---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Oauth Provers
  description: List configured OAuth providers.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth_providers:
    get:
      summary: Get Oauth Provers
      description: List configured OAuth providers.
      operationId: listOauthProviders_
      x-api-path-slug: oauth-providers-get
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---