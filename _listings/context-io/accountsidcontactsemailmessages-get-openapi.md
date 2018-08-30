---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Contacts Email Messages
  description: Lists messages where a contact is present. Returns the latest email
    messages exchanged with one or more email addresses. By "exchanged with Mr. X"
    we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both
    Mr. X and the mailbox owner.
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
  /connect_tokens:
    get:
      summary: Get Connect Tokens
      description: Lists connect tokens created with your API key.
      operationId: listConnectTokens_
      x-api-path-slug: connect-tokens-get
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
    post:
      summary: Post Connect Tokens
      description: Obtains a new connect_token.
      operationId: Create_obtainNewConnectToken_
      x-api-path-slug: connect-tokens-post
      parameters:
      - in: query
        name: callback_url
        description: When the users mailbox is connected to your API key, the browser
          will call this url (GET)
      - in: query
        name: email
        description: The email address of the account to be added
      - in: query
        name: first_name
        description: First name of the account holder
      - in: query
        name: last_name
        description: Last name of the account holder
      - in: query
        name: service_level
        description: Sets the service level of the accounts source to be created
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
  /connect_tokens/{token}:
    get:
      summary: Get Connect Tokens Token
      description: Gets information about a given connect token.
      operationId: getConnectToken_
      x-api-path-slug: connect-tokenstoken-get
      parameters:
      - in: path
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
      - Token
    delete:
      summary: Delete Connect Tokens Token
      description: Removes a given connect token.
      operationId: removeConnectToken_
      x-api-path-slug: connect-tokenstoken-delete
      parameters:
      - in: path
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
      - Token
  /accounts:
    get:
      summary: Get Accounts
      description: Lists accounts.
      operationId: listAccounts_
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: email
        description: Only return account associated to this email address
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: status
        description: Only return accounts with sources whose status is of a specific
          value
      - in: query
        name: status_ok
        description: Set to 0 to get all accounts with sources that are not working
          correctly
      - in: query
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Accounts
    post:
      summary: Post Accounts
      description: Adds a new account.
      operationId: addAccount_
      x-api-path-slug: accounts-post
      parameters:
      - in: query
        name: email
        description: The primary email address of the account holder
      - in: query
        name: first_name
        description: First name of the account holder
      - in: query
        name: last_name
        description: Last name of the account holder
      - in: query
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}:
    get:
      summary: Get Accounts
      description: Gets details about a given account.
      operationId: getAccount_
      x-api-path-slug: accountsid-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
    put:
      summary: Put Accounts
      description: Modifies a given account.
      operationId: modifyAccount_
      x-api-path-slug: accountsid-put
      parameters:
      - in: query
        name: first_name
        description: First name of the account holder
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: last_name
        description: Last name of the account holder
      responses:
        200:
          description: OK
      tags:
      - Accounts
    delete:
      summary: Delete Accounts
      description: Removes a given account.
      operationId: removeAccount_
      x-api-path-slug: accountsid-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}/connect_tokens:
    get:
      summary: Get Accounts Connect Tokens
      description: Lists connect tokens created for an account.
      operationId: listAccountConnectTokens_
      x-api-path-slug: accountsidconnect-tokens-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
    post:
      summary: Post Accounts Connect Tokens
      description: Obtains a new connect_token for a specific account.
      operationId: Create_obtainNewAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokens-post
      parameters:
      - in: query
        name: callback_url
        description: When the users mailbox is connected to your API key, the browser
          will call this url (GET)
      - in: query
        name: email
        description: The email address of the account to be added
      - in: query
        name: first_name
        description: First name of the account holder
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: last_name
        description: Last name of the account holder
      - in: query
        name: service_level
        description: Sets the service level of the accounts source to be created
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
  /accounts/{id}/connect_tokens/{token}:
    get:
      summary: Get Accounts Connect Tokens Token
      description: Gets information about a given connect token.
      operationId: getAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokenstoken-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: token
        description: The unique random token used to add a second source to an existing
          account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
      - Token
    delete:
      summary: Delete Accounts Connect Tokens Token
      description: Remove a given connect token.
      operationId: removeAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokenstoken-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: token
        description: The unique random token used to add a second source to an existing
          account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
      - Token
  /accounts/{id}/contacts:
    get:
      summary: Get Accounts Contacts
      description: Lists contacts in an account.
      operationId: listAccountContacts_
      x-api-path-slug: accountsidcontacts-get
      parameters:
      - in: query
        name: active_after
        description: Only include contacts included in at least one email dated after
          a given time
      - in: query
        name: active_before
        description: Only include contacts included in at least one email dated before
          a given time
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: search
        description: String identifying the name or the email address of the contact(s)
          you are looking for
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
  /accounts/{id}/contacts/{email}:
    get:
      summary: Get Accounts Contacts Email
      description: Gets information about a given contact.
      operationId: getAccountContact_
      x-api-path-slug: accountsidcontactsemail-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
  /accounts/{id}/contacts/{email}/files:
    get:
      summary: Get Accounts Contacts Email Files
      description: Lists files exchanged with a contact. Returns the latest attachments
        exchanged with one or more email addresses. By "exchanged with Mr. X" we mean
        any file attached to an email received from Mr. X, sent to Mr. X or sent by
        anyone to both Mr. X and the mailbox owner.
      operationId: listAccountContactFiles_
      x-api-path-slug: accountsidcontactsemailfiles-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Files
  /accounts/{id}/contacts/{email}/messages:
    get:
      summary: Get Accounts Contacts Email Messages
      description: Lists messages where a contact is present. Returns the latest email
        messages exchanged with one or more email addresses. By "exchanged with Mr.
        X" we mean any email received from Mr. X, sent to Mr. X or sent by anyone
        to both Mr. X and the mailbox owner.
      operationId: listAccountContactMessages_
      x-api-path-slug: accountsidcontactsemailmessages-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Messages
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