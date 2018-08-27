---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Patch Scopes Requests Request  Approve
  description: |-
    This endpoint allows you to approve an access attempt.

    **Note:** Only teammate admins may approve another teammate???s access request.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /scopes/requests/{request_id}/approve:
    patch:
      summary: Patch Scopes Requests Request  Approve
      description: |-
        This endpoint allows you to approve an access attempt.

        **Note:** Only teammate admins may approve another teammate???s access request.
      operationId: scopes.requests.request_id.approve.patch
      x-api-path-slug: scopesrequestsrequest-idapprove-patch
      responses:
        200:
          description: OK
      tags:
      - Email
      - Scopes
      - Requests
      - Request
      - ""
      - Approve
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