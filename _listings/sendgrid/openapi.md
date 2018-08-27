swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
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