swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts/dncs/sources/{source}:
    delete:
      summary: Delete do not contact (dnc) numbers contained in source.
      description: Delete Do Not Contact (DNC) contact entries contained in source.
      operationId: deleteDoNotContactsBySource
      x-api-path-slug: contactsdncssourcessource-delete
      parameters:
      - in: path
        name: source
        description: Source associated with Do Not Contact (DNC) entry
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Sources
      - Source