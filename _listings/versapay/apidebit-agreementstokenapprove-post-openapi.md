---
swagger: "2.0"
x-collection-name: VersaPay
x-complete: 0
info:
  title: VersaPay Approve an Agreement
  description: Approve an agreement.
  contact:
    name: VersaPay Support
    url: https://www.versapay.com/support
    email: support@versapay.com
  version: 1.0.0
host: secure.versapay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/transactions/{token}/approve:
    post:
      summary: Approve a Transaction
      description: |-
        Approve a `new` or `wait_for_request_approval` transaction.<br>
        An API key with administrative access is required to approve a transaction.
      operationId: approveTransaction
      x-api-path-slug: apitransactionstokenapprove-post
      parameters:
      - in: body
        name: fund_token
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: token
        description: The transaction identifier
      responses:
        200:
          description: OK
      tags:
      - Approve
      - Transactions
  /api/debit_agreements/{token}/approve:
    post:
      summary: Approve an Agreement
      description: Approve an agreement.
      operationId: approveAgreement
      x-api-path-slug: apidebit-agreementstokenapprove-post
      parameters:
      - in: body
        name: fund_token
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: token
        description: The agreement identifier
      responses:
        200:
          description: OK
      tags:
      - Approve
      - Agreements
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