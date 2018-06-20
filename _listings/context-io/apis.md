---
name: Context.IO
x-slug: context-io
description: Create simple email webhooks and code against a free, RESTful, IMAP API.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
x-kinRank: "9"
x-alexaRank: "569975"
tags: Context.IO
created: "2018-06-19"
modified: "2018-06-19"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/apis.md
specificationVersion: "0.14"
apis:
- name: Context.IO Get Oauth Provers
  x-api-slug: context-io
  description: List configured OAuth providers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///oauth_providers
  tags: Oauth,Providers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/oauth-providers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/oauth-providers-get-openapi.md
- name: Context.IO Post Oauth Provers
  x-api-slug: context-io
  description: Adds a new OAuth provider.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///oauth_providers
  tags: Oauth,Providers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/oauth-providers-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/oauth-providers-post-openapi.md
- name: Context.IO Get Oauth Provers Key
  x-api-slug: context-io
  description: Gets information about a given OAuth provider.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///oauth_providers/{key}
  tags: Oauth,Providers,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/oauth-providerskey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/oauth-providerskey-get-openapi.md
- name: Context.IO Delete Oauth Provers Key
  x-api-slug: context-io
  description: Removes a given OAuth provider.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///oauth_providers/{key}
  tags: Oauth,Providers,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/oauth-providerskey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/oauth-providerskey-delete-openapi.md
- name: Context.IO Get Discovery
  x-api-slug: context-io
  description: Attempts to discover IMAP settings for a given email address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///discovery
  tags: Discovery
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/discovery-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/discovery-get-openapi.md
- name: Context.IO Get Connect Tokens
  x-api-slug: context-io
  description: Lists connect tokens created with your API key.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///connect_tokens
  tags: Connect,Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/connect-tokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/connect-tokens-get-openapi.md
- name: Context.IO Post Connect Tokens
  x-api-slug: context-io
  description: Obtains a new connect_token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///connect_tokens
  tags: Connect,Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/connect-tokens-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/connect-tokens-post-openapi.md
- name: Context.IO Get Connect Tokens Token
  x-api-slug: context-io
  description: Gets information about a given connect token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///connect_tokens/{token}
  tags: Connect,Tokens,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/connect-tokenstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/connect-tokenstoken-get-openapi.md
- name: Context.IO Delete Connect Tokens Token
  x-api-slug: context-io
  description: Removes a given connect token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///connect_tokens/{token}
  tags: Connect,Tokens,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/connect-tokenstoken-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/connect-tokenstoken-delete-openapi.md
- name: Context.IO Get Accounts
  x-api-slug: context-io
  description: Lists accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts
  tags: Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accounts-get-openapi.md
- name: Context.IO Post Accounts
  x-api-slug: context-io
  description: Adds a new account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts
  tags: Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accounts-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accounts-post-openapi.md
- name: Context.IO Get Accounts
  x-api-slug: context-io
  description: Gets details about a given account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}
  tags: Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsid-get-openapi.md
- name: Context.IO Put Accounts
  x-api-slug: context-io
  description: Modifies a given account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}
  tags: Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsid-put-openapi.md
- name: Context.IO Delete Accounts
  x-api-slug: context-io
  description: Removes a given account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}
  tags: Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsid-delete-openapi.md
- name: Context.IO Get Accounts Connect Tokens
  x-api-slug: context-io
  description: Lists connect tokens created for an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/connect_tokens
  tags: Accounts,Connect,Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidconnect-tokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidconnect-tokens-get-openapi.md
- name: Context.IO Post Accounts Connect Tokens
  x-api-slug: context-io
  description: Obtains a new connect_token for a specific account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/connect_tokens
  tags: Accounts,Connect,Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidconnect-tokens-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidconnect-tokens-post-openapi.md
- name: Context.IO Get Accounts Connect Tokens Token
  x-api-slug: context-io
  description: Gets information about a given connect token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/connect_tokens/{token}
  tags: Accounts,Connect,Tokens,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidconnect-tokenstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidconnect-tokenstoken-get-openapi.md
- name: Context.IO Delete Accounts Connect Tokens Token
  x-api-slug: context-io
  description: Remove a given connect token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/connect_tokens/{token}
  tags: Accounts,Connect,Tokens,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidconnect-tokenstoken-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidconnect-tokenstoken-delete-openapi.md
- name: Context.IO Get Accounts Contacts
  x-api-slug: context-io
  description: Lists contacts in an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts
  tags: Accounts,Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontacts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontacts-get-openapi.md
- name: Context.IO Get Accounts Contacts Email
  x-api-slug: context-io
  description: Gets information about a given contact.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts/{email}
  tags: Accounts,Contacts,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontactsemail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontactsemail-get-openapi.md
- name: Context.IO Get Accounts Contacts Email Files
  x-api-slug: context-io
  description: Lists files exchanged with a contact. Returns the latest attachments
    exchanged with one or more email addresses. By "exchanged with Mr. X" we mean
    any file attached to an email received from Mr. X, sent to Mr. X or sent by anyone
    to both Mr. X and the mailbox owner.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts/{email}/files
  tags: Accounts,Contacts,Email,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontactsemailfiles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontactsemailfiles-get-openapi.md
- name: Context.IO Get Accounts Contacts Email Messages
  x-api-slug: context-io
  description: Lists messages where a contact is present. Returns the latest email
    messages exchanged with one or more email addresses. By "exchanged with Mr. X"
    we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both
    Mr. X and the mailbox owner.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts/{email}/messages
  tags: Accounts,Contacts,Email,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontactsemailmessages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontactsemailmessages-get-openapi.md
- name: Context.IO Get Accounts Contacts Email Threads
  x-api-slug: context-io
  description: Lists threads where a contact is present. Returns the latest email
    threads exchanged with one or more email addresses. By "exchanged with Mr. X"
    we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both
    Mr. X and the mailbox owner.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/contacts/{email}/threads
  tags: Accounts,Contacts,Email,Threads
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontactsemailthreads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidcontactsemailthreads-get-openapi.md
- name: Context.IO Get Accounts Email Addresses
  x-api-slug: context-io
  description: Lists email addresses used by an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/email_addresses
  tags: Accounts,Email,Addresses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidemail-addresses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidemail-addresses-get-openapi.md
- name: Context.IO Post Accounts Email Addresses
  x-api-slug: context-io
  description: Adds a new email address as an alias for an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/email_addresses
  tags: Accounts,Email,Addresses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidemail-addresses-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidemail-addresses-post-openapi.md
- name: Context.IO Post Accounts Email Addresses Email
  x-api-slug: context-io
  description: Makes this email address the primary one for the account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/email_addresses/{email}
  tags: Accounts,Email,Addresses,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidemail-addressesemail-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidemail-addressesemail-post-openapi.md
- name: Context.IO Delete Accounts Email Addresses Email
  x-api-slug: context-io
  description: Removes an email address form the aliases of an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/email_addresses/{email}
  tags: Accounts,Email,Addresses,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidemail-addressesemail-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidemail-addressesemail-delete-openapi.md
- name: Context.IO Get Accounts Files
  x-api-slug: context-io
  description: 'Lists files found as email attachments. List filters: each of the
    email, to, from, cc and bcc parameters can be set to a comma-separated list of
    email addresses. These multiple addresses are treated as an OR combination. You
    can set more than one parameter when doing this call. Multiple parameters are
    treated as an AND combination.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/files
  tags: Accounts,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfiles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfiles-get-openapi.md
- name: Context.IO Get Accounts Files Fileid
  x-api-slug: context-io
  description: Gets information about a given file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/files/{fileId}
  tags: Accounts,Files,FileId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileid-get-openapi.md
- name: Context.IO Get Accounts Files Fileid Changes
  x-api-slug: context-io
  description: Lists files that can be compared with a given file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/files/{fileId}/changes
  tags: Accounts,Files,FileId,Changes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileidchanges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileidchanges-get-openapi.md
- name: Context.IO Get Accounts Files Fileid Content
  x-api-slug: context-io
  description: 'Downloads a given file. Returns the content a given attachment. On-demand
    data retrieval: since we do not keep full copies of attachments on our servers,
    the file has to be retrieved from the IMAP server when this call is made. If the
    IMAP server is unreachable at the time the call is made, this call will return
    an error.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/files/{fileId}/content
  tags: Accounts,Files,FileId,Content
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileidcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileidcontent-get-openapi.md
- name: Context.IO Get Accounts Files Fileid Related
  x-api-slug: context-io
  description: Lists other files related to a given file. Returns a list of files
    that are related to the given file. Currently, relation between files is based
    on how similar their names are.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/files/{fileId}/related
  tags: Accounts,Files,FileId,Related
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileidrelated-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileidrelated-get-openapi.md
- name: Context.IO Get Accounts Files Fileid Revisions
  x-api-slug: context-io
  description: Lists other revisions of a given file. Returns a list of revisions
    attached to other emails in the mailbox for a given file. Two files are considered
    revisions of the same document if their file names are identical outside of revision
    indicators such as dates, author initials, version numbers and keywords like "final"
    or "draft".
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/files/{fileId}/revisions
  tags: Accounts,Files,FileId,Revisions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileidrevisions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidfilesfileidrevisions-get-openapi.md
- name: Context.IO Get Accounts Messages
  x-api-slug: context-io
  description: 'Lists email messages for an account. List filters: each of the email,
    to, from, cc and bcc parameters can be set to a comma-separated list of email
    addresses. These multiple addresses are treated as an OR combination. You can
    set more than one parameter when doing this call. Multiple parameters are treated
    as an AND combination.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages
  tags: Accounts,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessages-get-openapi.md
- name: Context.IO Get Accounts Messages Message
  x-api-slug: context-io
  description: Gets the file, contact and other information about a given email message.
    As specified in the RFC822, the < and > at the beginning and end of the Message-ID
    are part of the value and should be included if you're putting an email_message_id
    in the url.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages/{message_id}
  tags: Accounts,Messages,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-id-get-openapi.md
- name: Context.IO Post Accounts Messages Message
  x-api-slug: context-io
  description: Copies or moves a message. Allows you to copy or move a message between
    folders. If there are more than one sources on the account, you can use this call
    to copy/move the message between these sources. In this case, the dst_label parameter
    must identify the source you want to message to be copied/moved to.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages/{message_id}
  tags: Accounts,Messages,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-id-post-openapi.md
- name: Context.IO Get Accounts Messages Message Body
  x-api-slug: context-io
  description: 'Fetches the message body of a given email. On-demand data retrieval:
    since we do not keep full copies of emails on our servers, this call triggers
    a connection to the IMAP server to fetch the message. One thing to point out is
    we do fetch messages in such a way that large files attached to a message won''t
    make any difference in the response time. This call only returns text portions
    of messages, attachments aren''t included. To get a list of attachments on the
    message, look for the files property in the response of a message instance. To
    download the content of these attachments, use the files/content call.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages/{message_id}/body
  tags: Accounts,Messages,Message,Body
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idbody-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idbody-get-openapi.md
- name: Context.IO Get Accounts Messages Message Source
  x-api-slug: context-io
  description: 'Fetches the message source. Returns the raw RFC-822 message source
    for the message (including attachments) with no parsing or decoding to any portions
    of the message. On-demand data retrieval: since we do not keep full copies of
    emails on our servers, this call triggers a connection to the IMAP server to fetch
    the message. Attachments are part of the message source so they will impact how
    fast this call responds.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages/{message_id}/source
  tags: Accounts,Messages,Message,Source
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idsource-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idsource-get-openapi.md
- name: Context.IO Get Accounts Messages Message Flags
  x-api-slug: context-io
  description: 'Lists message flags for an account. On-demand data retrieval: to ensure
    up-to-date values, flags are not cached by Context.IO. This call triggers a connection
    to the IMAP server to fetch the current message flags before it returns.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages/{message_id}/flags
  tags: Accounts,Messages,Message,Flags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idflags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idflags-get-openapi.md
- name: Context.IO Post Accounts Messages Message Flags
  x-api-slug: context-io
  description: Sets message flags for a given email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages/{message_id}/flags
  tags: Accounts,Messages,Message,Flags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idflags-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idflags-post-openapi.md
- name: Context.IO Get Accounts Messages Message Headers
  x-api-slug: context-io
  description: 'Lists complete headers of a given email message. On-demand data retrieval:
    since we do not keep full copies of emails on our servers, this call triggers
    a connection to the IMAP server to fetch the message headers.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages/{message_id}/headers
  tags: Accounts,Messages,Message,Headers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idheaders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idheaders-get-openapi.md
- name: Context.IO Get Accounts Messages Message Thread
  x-api-slug: context-io
  description: Gets information about all messages of the thread a given message is
    in. This returns an array with the same structure as getting information on a
    single message for every message in the thread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/messages/{message_id}/thread
  tags: Accounts,Messages,Message,Thread
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idthread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidmessagesmessage-idthread-get-openapi.md
- name: Context.IO Get Accounts Sources
  x-api-slug: context-io
  description: Lists IMAP sources assigned for an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources
  tags: Accounts,Sources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsources-get-openapi.md
- name: Context.IO Post Accounts Sources
  x-api-slug: context-io
  description: Adds an IMAP account to a given account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources
  tags: Accounts,Sources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsources-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsources-post-openapi.md
- name: Context.IO Get Accounts Sources Label
  x-api-slug: context-io
  description: Gets parameters and status for an IMAP source.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources/{label}
  tags: Accounts,Sources,Label
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabel-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabel-get-openapi.md
- name: Context.IO Put Accounts Sources Label
  x-api-slug: context-io
  description: Modifies a data source on a given account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources/{label}
  tags: Accounts,Sources,Label
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabel-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabel-put-openapi.md
- name: Context.IO Delete Accounts Sources Label
  x-api-slug: context-io
  description: Removes a data source of an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources/{label}
  tags: Accounts,Sources,Label
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabel-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabel-delete-openapi.md
- name: Context.IO Get Accounts Sources Label Folders
  x-api-slug: context-io
  description: Lists folders in an IMAP source. Returns folders existing in a given
    IMAP account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources/{label}/folders
  tags: Accounts,Sources,Label,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabelfolders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabelfolders-get-openapi.md
- name: Context.IO Put Accounts Sources Label Folders Folder
  x-api-slug: context-io
  description: |-
    Creates a folder on an IMAP source. A new folder can be added to an IMAP source by PUTting the desired path under the sources/folders resource.
    Working with server-specific hierarchy delimiters:
    IMAP servers are free to use the character they want as the folder hierarchy delimiter. The bad news is they don't use the same. The good news is you don't need to know this, we take care of it.

    Then what is that delim parameter for?
    Good question. By default, we expect you to specify the folder hierarchy using / as the hierarchy delimiter. For example, to create a folder called my folder under the folder base folder, you would call:
    PUT /2.0/accounts/<id>/sources/<label>/folders/base+folder/my+folder

    No matter what's the actual hierarchy delimiter the IMAP server expects, this call will work. However, say you need to use another character as the delimiter, here's how you'd do it:
    PUT /2.0/accounts/<id>/sources/<label>/folders/base+folder.my+folder?delim=.

    Both examples above are equivalent and will have the same result no matter what the IMAP server expects as the actual hierarchy delimiter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources/{label}/folders/{folder}
  tags: Accounts,Sources,Label,Folders,Folder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabelfoldersfolder-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabelfoldersfolder-put-openapi.md
- name: Context.IO Get Accounts Sources Label Sync
  x-api-slug: context-io
  description: Gets the sync status of a data source. Returns the timestamps for the
    last time the source has been synced with the origin mailbox.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources/{label}/sync
  tags: Accounts,Sources,Label,Sync
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabelsync-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabelsync-get-openapi.md
- name: Context.IO Post Accounts Sources Label Sync
  x-api-slug: context-io
  description: Triggers a sync of a data source. This will start a sync job for the
    source.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sources/{label}/sync
  tags: Accounts,Sources,Label,Sync
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabelsync-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsourceslabelsync-post-openapi.md
- name: Context.IO Get Accounts Sync
  x-api-slug: context-io
  description: Gets the sync status for all sources of the account. Returns the timestamps
    for the last time a source has been synced with the origin mailbox.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sync
  tags: Accounts,Sync
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsync-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsync-get-openapi.md
- name: Context.IO Post Accounts Sync
  x-api-slug: context-io
  description: Triggers a sync of all sources on the account. This will start a sync
    job for all sources under the account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/sync
  tags: Accounts,Sync
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsync-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidsync-post-openapi.md
- name: Context.IO Get Accounts Threads
  x-api-slug: context-io
  description: Lists threads on an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/threads
  tags: Accounts,Threads
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidthreads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidthreads-get-openapi.md
- name: Context.IO Get Accounts Threads Thread
  x-api-slug: context-io
  description: |-
    Returns files, contacts and messages on a given thread. The purpose is to allow Gmail extensions to easily retrieve data when users's load a conversation in the Gmail UI. Hence, threads are identified by the value of their Gmail thread prefixed with "gm-".
    For example, if the URL of a conversation in the Gmail UI is https://mail.google.com/mail/u/0/#mbox/13119ab37f00b826, you would obtain the details about this thread by calling:
    GET https://api.context.io/2.0/accounts/<accountId>/threads/gm-13119ab37f00b826

    What about threads on non-Gmail mailboxes?
    You can retrieve thread information for any message using the Thread resource of that message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/threads/{thread_id}
  tags: Accounts,Threads,Thread
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidthreadsthread-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidthreadsthread-id-get-openapi.md
- name: Context.IO Get Accounts Webhooks
  x-api-slug: context-io
  description: List WebHooks configured for an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/webhooks
  tags: Accounts,Webhooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhooks-get-openapi.md
- name: Context.IO Post Accounts Webhooks
  x-api-slug: context-io
  description: Creates a new WebHook on an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/webhooks
  tags: Accounts,Webhooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhooks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhooks-post-openapi.md
- name: Context.IO Get Accounts Webhooks Webhook
  x-api-slug: context-io
  description: Gets properties of a given WebHook.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/webhooks/{webhook_id}
  tags: Accounts,Webhooks,Webhook
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhookswebhook-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhookswebhook-id-get-openapi.md
- name: Context.IO Post Accounts Webhooks Webhook
  x-api-slug: context-io
  description: |-
    Changes properties of a given WebHook. The only property of a WebHook that can be changed is it's active property. If you want to change the filters or callback urls, delete it and create a new one.
    Changing the active property can be useful in two cases:
    - Pause/resume WebHooks: If your application needs up-to-date information when users are logged in the best option is to keep a WebHook with no filters on that account that will be resumed (setting active to 1) when the user logs in and paused (setting active to 0) when the user logs out of your app.
    - Acting upon a failure notification: If a WebHook fails, your failure_notif_url is called (see creating a WebHook) an its active property becomes 0. Set the active property back to 1 to get it working again.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/webhooks/{webhook_id}
  tags: Accounts,Webhooks,Webhook
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhookswebhook-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhookswebhook-id-post-openapi.md
- name: Context.IO Delete Accounts Webhooks Webhook
  x-api-slug: context-io
  description: Cancels a WebHook.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/webhooks/{webhook_id}
  tags: Accounts,Webhooks,Webhook
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhookswebhook-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/accountsidwebhookswebhook-id-delete-openapi.md
- name: Context.IO
  x-api-slug: context-io
  description: Context.IO is the missing email API that makes it easy and fastto integrate
    your users email data in your application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: Context.IO
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/context-io/master/_listings/context-io/openapi.md
x-common:
- type: x-base
  url: https://api.context.io/
- type: x-blog
  url: http://blog.context.io/
- type: x-blog-rss
  url: http://blog.context.io/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/product/context-io
- type: x-crunchbase
  url: https://crunchbase.com/organization/context-io
- type: x-documentation
  url: http://context.io/docs/2.0
- type: x-email
  url: hello@context.io
- type: x-email
  url: support@context.io
- type: x-email
  url: business@context.io
- type: x-faq
  url: http://context.io/privacy-faq
- type: x-github
  url: https://github.com/contextio
- type: x-ios-library
  url: https://github.com/contextio/contextio-ios
- type: x-node-js-library
  url: https://github.com/contextio/ContextIO-node
- type: x-php-library
  url: https://github.com/contextio/PHP-ContextIO
- type: x-pricing
  url: http://context.io/pricing
- type: x-privacy
  url: http://www.returnpath.com/privacy-policy-data
- type: x-python-library
  url: https://github.com/contextio/Python-ContextIO
- type: x-ruby-library
  url: https://github.com/contextio/contextio-ruby
- type: x-selfservice-registration
  url: http://context.io/#signup
- type: x-terms-of-service
  url: http://context.io/terms-of-service
- type: x-twitter
  url: https://twitter.com/contextio
- type: x-website
  url: http://context.io/
- type: x-website
  url: http://context.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---