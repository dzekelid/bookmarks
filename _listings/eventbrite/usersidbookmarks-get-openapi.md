---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Users Bookmarks
  description: Gets all the user&#8217;s saved events.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}/bookmarks/:
    get:
      summary: Get Users Bookmarks
      description: Gets all the user&#8217;s saved events.
      operationId: getUsersBookmarks
      x-api-path-slug: usersidbookmarks-get
      parameters:
      - in: query
        name: bookmark_list_id
        description: Optional bookmark list id to fetch all bookmarks from
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Bookmarks
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