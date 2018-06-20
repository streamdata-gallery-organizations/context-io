---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Discovery
  description: Attempts to discover IMAP settings for a given email address.
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
    post:
      summary: Post Oauth Provers
      description: Adds a new OAuth provider.
      operationId: addOauthProviders_
      x-api-path-slug: oauth-providers-post
      parameters:
      - in: query
        name: provider_consumer_key
        description: The OAuth consumer key
      - in: query
        name: provider_consumer_secret
        description: The OAuth consumer secret
      - in: query
        name: type
        description: Identification of the OAuth provider
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
  /oauth_providers/{key}:
    get:
      summary: Get Oauth Provers Key
      description: Gets information about a given OAuth provider.
      operationId: getOauthProvider_
      x-api-path-slug: oauth-providerskey-get
      parameters:
      - in: path
        name: key
        description: The consumer key for this external OAuth provider
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
      - Key
    delete:
      summary: Delete Oauth Provers Key
      description: Removes a given OAuth provider.
      operationId: removeOauthProvider_
      x-api-path-slug: oauth-providerskey-delete
      parameters:
      - in: path
        name: key
        description: The consumer key for this external OAuth provider
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
      - Key
  /discovery:
    get:
      summary: Get Discovery
      description: Attempts to discover IMAP settings for a given email address.
      operationId: Get_discoverEmailImapSettings_
      x-api-path-slug: discovery-get
      parameters:
      - in: query
        name: email
        description: An email address you want to discover IMAP settings for
      - in: query
        name: source_type
        description: The type of source you want to discover settings for
      responses:
        200:
          description: OK
      tags:
      - Discovery
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