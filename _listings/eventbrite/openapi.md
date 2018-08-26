---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
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
  /users/{id}/bookmarks/unsave/:
    post:
      summary: Post Users Bookmarks Unsave
      description: 'Removes the specified bookmark from the event for the user. Returns
        {&quot;deleted&quot;: true}.'
      operationId: postUsersBookmarksUnsave
      x-api-path-slug: usersidbookmarksunsave-post
      parameters:
      - in: query
        name: bookmark_list_id
        description: Bookmark list id to save the bookmark(s) to
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
      - Unsave
---