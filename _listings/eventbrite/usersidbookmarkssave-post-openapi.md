---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Post Users Bookmarks Save
  description: 'Adds a new bookmark for the user. Returns {&quot;created&quot;: true}.'
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
  /users/{id}/bookmarks/save/:
    post:
      summary: Post Users Bookmarks Save
      description: 'Adds a new bookmark for the user. Returns {&quot;created&quot;:
        true}.'
      operationId: postUsersBookmarksSave
      x-api-path-slug: usersidbookmarkssave-post
      parameters:
      - in: query
        name: bookmark_list_id
        description: Optional Bookmark list id to save the bookmark(s) to
        type: query
      - in: query
        name: event_id
        description: Event id to bookmark for the user
        type: query
      - in: query
        name: event_ids
        description: Event ids to batch bookmark for the user
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Bookmarks
      - Save
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