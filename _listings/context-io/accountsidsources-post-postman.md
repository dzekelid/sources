{
  "info": {
    "name": "Context.IO Post Accounts Sources",
    "_postman_id": "8231d251-1c9a-4232-bf02-70a6d140c34a",
    "description": "Adds an IMAP account to a given account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "bae791da-6945-4d0f-a1fd-d030fc49315e",
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
              "id": "dff820e5-9690-4569-957e-bfa2a4d46a30"
            }
          ]
        },
        {
          "id": "0ef8321d-4e32-4c56-9f9b-c0cba9fb3b94",
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
              "id": "257a1d48-0d25-41f3-a0cb-1c24bbfa5fff"
            }
          ]
        },
        {
          "id": "9264e6ff-94bd-4e97-9a7f-1421ebe84de3",
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
              "id": "3dd10b39-bbd5-49ba-8b8a-a6cf994dce62"
            }
          ]
        },
        {
          "id": "f8acb75d-9c32-4536-a0ee-852c734f5e68",
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
              "id": "5c637af3-5c7d-4a2a-9d9a-b01c06f2eec1"
            }
          ]
        },
        {
          "id": "f5d51b24-aa4b-4a5f-a338-cd9583e83058",
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
              "id": "69a65878-9ff0-4401-bf55-e6f12ef0feca"
            }
          ]
        },
        {
          "id": "5635a4f9-f939-49e2-9292-648a3366970d",
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
              "id": "3f573746-f4f0-48b7-8655-b70cb53818be"
            }
          ]
        },
        {
          "id": "8e7ee4b4-1532-45ee-afa9-d737329523a1",
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
              "id": "18a3e8ed-0f0b-45a7-8d59-500ef38e0f57"
            }
          ]
        },
        {
          "id": "9114f05c-b660-42ac-a4b4-0a3292f059de",
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
              "id": "35d33937-9613-47da-bc6d-4e26991a1cdc"
            }
          ]
        },
        {
          "id": "d716aa42-4123-40d7-a4f4-9f258aa17bde",
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
              "id": "3b2bc5f5-6518-4991-af0b-ed97ef1c6dd7"
            }
          ]
        },
        {
          "id": "86d24367-0933-4a86-bcf1-bd5d0873fb17",
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
              "id": "793a80fb-b3ac-469a-a1ba-f8049b257e0b"
            }
          ]
        },
        {
          "id": "91efb990-06a7-4d90-8e40-4daf68b5b3a1",
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
              "id": "e58c067c-a7ca-4a15-ab32-9143e066a10b"
            }
          ]
        },
        {
          "id": "98c98102-3fe6-4e23-be82-749564db3fda",
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
              "id": "5251f5e0-70ff-4f9e-9f59-4b9f6f6ecc2b"
            }
          ]
        },
        {
          "id": "f58014a5-a4f1-46e6-afdf-9f772cccaab5",
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
              "id": "74910e90-02d5-471a-99ee-315e480239fb"
            }
          ]
        },
        {
          "id": "fd471ed0-7d93-4994-95aa-bc3c09484284",
          "name": "listAccountContactThreads_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/contacts/:email/threads"
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
            "description": "Lists threads where a contact is present. Returns the latest email threads exchanged with one or more email addresses. By \"exchanged with Mr. X\" we mean any email received from Mr. X, sent to Mr. X or sent by anyone to both Mr. X and the mailbox owner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6e3d322-2fc7-402d-8c9d-012c268ff9a0"
            }
          ]
        },
        {
          "id": "fc2e92df-b4e0-4d27-95e8-a10eb1cbe836",
          "name": "listAccountEmailAddresses_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/email_addresses"
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
            "description": "Lists email addresses used by an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10d1fa1d-ab55-4504-ab1b-29f26599f575"
            }
          ]
        },
        {
          "id": "b45e5780-3a5a-4ea9-ba09-27835c344eaf",
          "name": "addAccountEmailAddress_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/email_addresses"
              ],
              "query": [
                {
                  "key": "email_address",
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
            "description": "Adds a new email address as an alias for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46b0997b-dcc6-4a1f-82d5-41baf8db0f2b"
            }
          ]
        },
        {
          "id": "fa2597c9-0909-4471-ad76-eb43890f8eba",
          "name": "Create_setAccountEmailAddressAsPrimary_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/email_addresses/:email"
              ],
              "query": [
                {
                  "key": "primary",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Makes this email address the primary one for the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db782600-8c8b-4947-9832-8e026d41345b"
            }
          ]
        },
        {
          "id": "37ea90e7-c60e-4035-b416-01c9c9262074",
          "name": "removeAccountEmailAddress_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/email_addresses/:email"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an email address form the aliases of an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0bded3b-3bd2-4fe5-9ff9-8369ab4eb254"
            }
          ]
        },
        {
          "id": "c0fedc4c-ead2-49cf-8533-94b285ae43ee",
          "name": "listAccountFiles_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files"
              ],
              "query": [
                {
                  "key": "bcc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "cc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "file_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_by_revisions",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "indexed_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "indexed_before",
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
                  "key": "to",
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
            "description": "Lists files found as email attachments. List filters: each of the email, to, from, cc and bcc parameters can be set to a comma-separated list of email addresses. These multiple addresses are treated as an OR combination. You can set more than one parameter when doing this call. Multiple parameters are treated as an AND combination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e2ff013-14b3-4b54-a5c5-47109e977be1"
            }
          ]
        },
        {
          "id": "f567ae97-0eae-4c2f-b99f-4c400192f18a",
          "name": "getAccountFile_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId"
              ],
              "variable": [
                {
                  "id": "fileId",
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
            "description": "Gets information about a given file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77423147-4378-4c73-af22-af9a80c1ef36"
            }
          ]
        },
        {
          "id": "45b88743-e971-4d2d-842e-1c2e5a968670",
          "name": "listComparableAccountFiles_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId/changes"
              ],
              "variable": [
                {
                  "id": "fileId",
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
            "description": "Lists files that can be compared with a given file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7959513-e6f7-453a-89fe-3467e339999e"
            }
          ]
        },
        {
          "id": "5f642bc8-34eb-4a49-bd0d-60034b5952ff",
          "name": "getAccountFileContent_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId/content"
              ],
              "variable": [
                {
                  "id": "fileId",
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
            "description": "Downloads a given file. Returns the content a given attachment. On-demand data retrieval: since we do not keep full copies of attachments on our servers, the file has to be retrieved from the IMAP server when this call is made. If the IMAP server is unreachable at the time the call is made, this call will return an error."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab7fe51a-99ef-455a-9393-f8413b2e4200"
            }
          ]
        },
        {
          "id": "d4ba5c74-7c67-43c2-9042-4416613efb21",
          "name": "listAccountFileRelatedFiles_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId/related"
              ],
              "variable": [
                {
                  "id": "fileId",
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
            "description": "Lists other files related to a given file. Returns a list of files that are related to the given file. Currently, relation between files is based on how similar their names are."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3633821e-b7ec-4e9b-8ce4-8e010a84407a"
            }
          ]
        },
        {
          "id": "965ccc45-f853-4247-8f62-e4d1207cfd0a",
          "name": "listAccountFileRevisions_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/files/:fileId/revisions"
              ],
              "variable": [
                {
                  "id": "fileId",
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
            "description": "Lists other revisions of a given file. Returns a list of revisions attached to other emails in the mailbox for a given file. Two files are considered revisions of the same document if their file names are identical outside of revision indicators such as dates, author initials, version numbers and keywords like \"final\" or \"draft\"."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93dd98f6-6fab-4028-8ad2-f8641915549a"
            }
          ]
        },
        {
          "id": "6aabb3fb-dcbb-41b6-8829-ee8fafae467e",
          "name": "listAccountMessages_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages"
              ],
              "query": [
                {
                  "key": "bcc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "body_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "cc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "folder",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_body",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_flags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_headers",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "indexed_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "indexed_before",
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
                  "key": "subject",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "to",
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
            "description": "Lists email messages for an account. List filters: each of the email, to, from, cc and bcc parameters can be set to a comma-separated list of email addresses. These multiple addresses are treated as an OR combination. You can set more than one parameter when doing this call. Multiple parameters are treated as an AND combination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b253e54b-b23f-4d15-8314-918a31745aa7"
            }
          ]
        },
        {
          "id": "1e62e1bb-4b0b-48e4-854b-19da7fa4ec95",
          "name": "getAccountMessage_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the file, contact and other information about a given email message. As specified in the RFC822, the < and > at the beginning and end of the Message-ID are part of the value and should be included if you're putting an email_message_id in the url."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24421cac-bb5f-4d18-8dfb-611f19862604"
            }
          ]
        },
        {
          "id": "c0e830ee-4475-4e9a-a77e-c343ed8db81d",
          "name": "Create_copyMoveAccountMessage_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id"
              ],
              "query": [
                {
                  "key": "dst_folder",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "dst_source",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "move",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Copies or moves a message. Allows you to copy or move a message between folders. If there are more than one sources on the account, you can use this call to copy/move the message between these sources. In this case, the dst_label parameter must identify the source you want to message to be copied/moved to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "975686c1-5f00-445b-a1fe-12d7c542cce3"
            }
          ]
        },
        {
          "id": "53a6c9fb-9b3a-4934-8439-12aae85252d1",
          "name": "getAccountMessageBody_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/body"
              ],
              "query": [
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the message body of a given email. On-demand data retrieval: since we do not keep full copies of emails on our servers, this call triggers a connection to the IMAP server to fetch the message. One thing to point out is we do fetch messages in such a way that large files attached to a message won't make any difference in the response time. This call only returns text portions of messages, attachments aren't included. To get a list of attachments on the message, look for the files property in the response of a message instance. To download the content of these attachments, use the files/content call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a74b749-e694-4e6c-baf8-a0f53f3f2e04"
            }
          ]
        },
        {
          "id": "e31fdbab-820c-463a-bbd5-ec560ea3f5ba",
          "name": "getAccountMessageSource_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/source"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the message source. Returns the raw RFC-822 message source for the message (including attachments) with no parsing or decoding to any portions of the message. On-demand data retrieval: since we do not keep full copies of emails on our servers, this call triggers a connection to the IMAP server to fetch the message. Attachments are part of the message source so they will impact how fast this call responds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83421f82-b6ea-4ff4-8acb-c0952edd2e6e"
            }
          ]
        },
        {
          "id": "00eb82b2-8af4-4dca-b906-d95428d24d08",
          "name": "listAccountMessageFlags_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/flags"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists message flags for an account. On-demand data retrieval: to ensure up-to-date values, flags are not cached by Context.IO. This call triggers a connection to the IMAP server to fetch the current message flags before it returns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c08fba0-0d5d-4504-a8f3-e51f063535d0"
            }
          ]
        },
        {
          "id": "bee35978-1176-4a3f-b763-0154600e8226",
          "name": "Create_setAccountMessageFlags_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/flags"
              ],
              "query": [
                {
                  "key": "answered",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "deleted",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "draft",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "flagged",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "seen",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets message flags for a given email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55c78b00-a28f-4eea-9a0f-6da0f3ad72aa"
            }
          ]
        },
        {
          "id": "a7a6c930-9488-4ce8-836c-4d4ad7079dff",
          "name": "listAccountMessageHeaders_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/headers"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists complete headers of a given email message. On-demand data retrieval: since we do not keep full copies of emails on our servers, this call triggers a connection to the IMAP server to fetch the message headers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0daab4e2-9950-49bc-9bbb-0d599c97f7be"
            }
          ]
        },
        {
          "id": "04529138-00f9-41a3-998f-f43a54538d2b",
          "name": "getAccountMessageThread_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/messages/:message_id/thread"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about all messages of the thread a given message is in. This returns an array with the same structure as getting information on a single message for every message in the thread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e33ead7-f6c1-4aa3-ba26-808d9d6fdcbf"
            }
          ]
        },
        {
          "id": "75d0e9f4-d22c-47fa-bc6b-09eb335e8e98",
          "name": "listAccountSources_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources"
              ],
              "query": [
                {
                  "key": "status",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status_ok",
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
            "description": "Lists IMAP sources assigned for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67385e14-d706-4152-a9e8-2f7e083760d8"
            }
          ]
        },
        {
          "id": "e366fc63-6c83-4515-8b9f-b4e6680c78af",
          "name": "addAccountSource_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.context.io",
              "path": [
                "2.0",
                "accounts/:id/sources"
              ],
              "query": [
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "password",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "port",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_consumer_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_token",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_token_secret",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "server",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "service_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sync_period",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "username",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "use_ssl",
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
            "description": "Adds an IMAP account to a given account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6ba684b-4342-4665-a0aa-a53e62b19f48"
            }
          ]
        }
      ]
    }
  ]
}