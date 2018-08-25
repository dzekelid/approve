---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/event/approve/{eventId}:
    post:
      summary: Post Admin Event Approve Eventid
      description: Post admin event approve eventid.
      operationId: postApiV1AdminEventApproveEvent
      x-api-path-slug: apiv1admineventapproveeventid-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Approve
      - Eventid
  /api/v1/managers/approve/{artistId}:
    post:
      summary: Post Managers Approve Artistid
      description: Post managers approve artistid.
      operationId: postApiV1ManagersApproveArtist
      x-api-path-slug: apiv1managersapproveartistid-post
      parameters:
      - in: path
        name: artistId
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Managers
      - Approve
      - Artistid
---