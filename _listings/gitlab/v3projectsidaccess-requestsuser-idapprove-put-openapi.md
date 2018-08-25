---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Put Projects Access Requests User Approve
  version: 1.0.0
  description: This feature was introduced in GitLab 8.11.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/groups/{id}/access_requests/{user_id}/approve:
    put:
      summary: Put Groups Access Requests User Approve
      description: This feature was introduced in GitLab 8.11.
      operationId: putV3GroupsIdAccessRequestsUserIdApprove
      x-api-path-slug: v3groupsidaccess-requestsuser-idapprove-put
      parameters:
      - in: formData
        name: access_level
        description: 'A valid access level (defaults: `30`, developer access level)'
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the access requester
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Access
      - Requests
      - User
      - Approve
  /v3/projects/{id}/access_requests/{user_id}/approve:
    put:
      summary: Put Projects Access Requests User Approve
      description: This feature was introduced in GitLab 8.11.
      operationId: putV3ProjectsIdAccessRequestsUserIdApprove
      x-api-path-slug: v3projectsidaccess-requestsuser-idapprove-put
      parameters:
      - in: formData
        name: access_level
        description: 'A valid access level (defaults: `30`, developer access level)'
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the access requester
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Access
      - Requests
      - User
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