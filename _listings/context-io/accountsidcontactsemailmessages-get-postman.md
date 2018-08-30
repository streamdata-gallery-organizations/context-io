{
  "info": {
    "name": "Context.IO Get Accounts Contacts Email Messages",
    "_postman_id": "436258c2-cb23-4d6e-b9f7-43aa7be34b30",
    "description": "Lists messages where a contact is present. Returns the latest email messages exchanged with one or more email addresses. By \"exchanged with Mr. X\" we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both Mr. X and the mailbox owner.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "29690ad8-2dfa-4c77-86f7-caae4f0caed5",
          "name": "listAccounts_",
          "request": {
            "url": "http://api.context.io/2.0/accounts?email=%7B%7D&limit=%7B%7D&offset=%7B%7D&status=%7B%7D&status_ok=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2fbbc84-11b2-4ee3-beb5-c97153cbb27f"
            }
          ]
        },
        {
          "id": "cd15efa7-9850-4ded-909a-fa9c5b7e7c77",
          "name": "addAccount_",
          "request": {
            "url": "http://api.context.io/2.0/accounts?email=%7B%7D&first_name=%7B%7D&last_name=%7B%7D&token=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe1d2449-f1e5-4596-9c8d-ef700682962e"
            }
          ]
        },
        {
          "id": "4c913417-6509-4166-a0b5-03eba7c492bc",
          "name": "getAccount_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details about a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6341b967-ac86-46a7-ab23-1bc910d72994"
            }
          ]
        },
        {
          "id": "cf043430-ef88-4860-b23b-0fca5ac4984a",
          "name": "modifyAccount_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id"
              ],
              "query": [
                {
                  "key": "first_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "last_name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8496c9df-4d55-41a9-a5ea-3b08f4a78d3e"
            }
          ]
        },
        {
          "id": "bdd575f0-942a-4852-bc0e-0a633b64d824",
          "name": "removeAccount_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3aa65680-99a1-4be8-a522-1fa8eda7094b"
            }
          ]
        },
        {
          "id": "68c4b552-4940-47b2-8f87-48ede7c00673",
          "name": "listAccountConnectTokens_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/connect_tokens"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists connect tokens created for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e539efe-4489-4181-8c2c-406eb446e20e"
            }
          ]
        },
        {
          "id": "a948d11e-96ef-4f80-8572-f3c4eb7a92ea",
          "name": "Create_obtainNewAccountConnectToken_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/connect_tokens"
              ],
              "query": [
                {
                  "key": "callback_url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "first_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "last_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "service_level",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains a new connect_token for a specific account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2fa81b1-fce7-4055-9bc2-598fc2dcd865"
            }
          ]
        },
        {
          "id": "cce5e98f-eab1-4a11-862d-11a7ddc185de",
          "name": "getAccountConnectToken_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/connect_tokens/:token"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
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
              "id": "fe63f458-eeac-406b-a94f-9b3e89a77592"
            }
          ]
        },
        {
          "id": "d7300f6f-0c65-4151-b87a-5522d3a1226a",
          "name": "removeAccountConnectToken_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/connect_tokens/:token"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Remove a given connect token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c58f39be-e4e3-4939-afb2-324a485f55bc"
            }
          ]
        },
        {
          "id": "3004d31b-5f65-4531-a235-579b8684d2ef",
          "name": "listAccountContacts_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts"
              ],
              "query": [
                {
                  "key": "active_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "active_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists contacts in an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "926e057a-b216-4658-ae0c-49351748b054"
            }
          ]
        },
        {
          "id": "5f09a38a-d665-4478-9683-0a40ae475bc7",
          "name": "getAccountContact_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts/:email"
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a given contact."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b866f67c-321f-468c-a4a8-76c01ea79ede"
            }
          ]
        },
        {
          "id": "9051c851-9e14-474d-9f72-8f21a710bb9b",
          "name": "listAccountContactFiles_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts/:email/files"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists files exchanged with a contact. Returns the latest attachments exchanged with one or more email addresses. By \"exchanged with Mr. X\" we mean any file attached to an email received from Mr. X, sent to Mr. X or sent by anyone to both Mr. X and the mailbox owner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb7d799d-1c0e-4107-8ba9-01a11cdd7cfa"
            }
          ]
        },
        {
          "id": "b32e32c7-f936-4932-a099-b796eb914a2c",
          "name": "listAccountContactMessages_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts/:email/messages"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists messages where a contact is present. Returns the latest email messages exchanged with one or more email addresses. By \"exchanged with Mr. X\" we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both Mr. X and the mailbox owner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30cb34b4-d5c3-49eb-83e2-2efb01144899"
            }
          ]
        }
      ]
    }
  ]
}