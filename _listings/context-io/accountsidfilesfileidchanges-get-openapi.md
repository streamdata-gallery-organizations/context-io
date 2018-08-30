---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Files Fileid Changes
  description: Lists files that can be compared with a given file.
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
  /accounts/{id}/contacts/{email}/threads:
    get:
      summary: Get Accounts Contacts Email Threads
      description: Lists threads where a contact is present. Returns the latest email
        threads exchanged with one or more email addresses. By "exchanged with Mr.
        X" we mean any email received from Mr. X, sent to Mr. X or sent by anyone
        to both Mr. X and the mailbox owner.
      operationId: listAccountContactThreads_
      x-api-path-slug: accountsidcontactsemailthreads-get
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
      - Threads
  /accounts/{id}/email_addresses:
    get:
      summary: Get Accounts Email Addresses
      description: Lists email addresses used by an account.
      operationId: listAccountEmailAddresses_
      x-api-path-slug: accountsidemail-addresses-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
    post:
      summary: Post Accounts Email Addresses
      description: Adds a new email address as an alias for an account.
      operationId: addAccountEmailAddress_
      x-api-path-slug: accountsidemail-addresses-post
      parameters:
      - in: query
        name: email_address
        description: An email address
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
  /accounts/{id}/email_addresses/{email}:
    post:
      summary: Post Accounts Email Addresses Email
      description: Makes this email address the primary one for the account.
      operationId: Create_setAccountEmailAddressAsPrimary_
      x-api-path-slug: accountsidemail-addressesemail-post
      parameters:
      - in: path
        name: email
        description: One of the email addresses associated to the account
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: primary
        description: Set to 1 to make this email address the primary one for the account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
      - Email
    delete:
      summary: Delete Accounts Email Addresses Email
      description: Removes an email address form the aliases of an account.
      operationId: removeAccountEmailAddress_
      x-api-path-slug: accountsidemail-addressesemail-delete
      parameters:
      - in: path
        name: email
        description: One of the email addresses associated to the account
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
      - Email
  /accounts/{id}/files:
    get:
      summary: Get Accounts Files
      description: 'Lists files found as email attachments. List filters: each of
        the email, to, from, cc and bcc parameters can be set to a comma-separated
        list of email addresses. These multiple addresses are treated as an OR combination.
        You can set more than one parameter when doing this call. Multiple parameters
        are treated as an AND combination.'
      operationId: listAccountFiles_
      x-api-path-slug: accountsidfiles-get
      parameters:
      - in: query
        name: bcc
        description: Email address of a contact BCCed on the messages
      - in: query
        name: cc
        description: Email address of a contact CCed on the messages
      - in: query
        name: date_after
        description: Only include files attached to messages sent after a given timestamp
      - in: query
        name: date_before
        description: Only include files attached to messages sent before a given timestamp
      - in: query
        name: email
        description: Email address of the contact for whom you want the latest files
          exchanged with
      - in: query
        name: file_name
        description: Search for files based on their name
      - in: query
        name: from
        description: Email address of a contact files have been received from
      - in: query
        name: group_by_revisions
        description: If set to 1, the list will do an intelligent grouping of files
          to reflect occurrences of the same document
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: indexed_after
        description: Only include files attached to messages indexed after a given
          timestamp
      - in: query
        name: indexed_before
        description: Only include files attached to messages indexed before a given
          timestamp
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: to
        description: Email address of a contact files have been sent to
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
  /accounts/{id}/files/{fileId}:
    get:
      summary: Get Accounts Files Fileid
      description: Gets information about a given file.
      operationId: getAccountFile_
      x-api-path-slug: accountsidfilesfileid-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
  /accounts/{id}/files/{fileId}/changes:
    get:
      summary: Get Accounts Files Fileid Changes
      description: Lists files that can be compared with a given file.
      operationId: listComparableAccountFiles_
      x-api-path-slug: accountsidfilesfileidchanges-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Changes
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