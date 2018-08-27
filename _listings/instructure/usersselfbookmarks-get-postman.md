{
  "info": {
    "name": "Instructure Canvas Users API List bookmarks",
    "_postman_id": "15663237-980b-44f5-8fac-1baee4881628",
    "description": "List bookmarks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "12640d61-1c4d-4c3d-82ed-f55ff210c0cc",
          "name": "list-the-activity-stream",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/activity_stream",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c1fb092-4ebb-4203-89f6-d1c8cc4d31ed"
            }
          ]
        },
        {
          "id": "a68785b9-c7bf-4386-a0a0-cabfe5d5777f",
          "name": "list-the-activity-stream1",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9bf4d37-0ba2-4c16-9732-66556d10827f"
            }
          ]
        },
        {
          "id": "282ab76f-3843-4b19-aba5-69bdbfa8777e",
          "name": "hide-all-stream-items",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Hide all stream items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a0713b7-dd7e-481b-8eb5-f28a734f01d7"
            }
          ]
        },
        {
          "id": "e7250475-18df-4643-a243-9785b1a0c3e7",
          "name": "activity-stream-summary",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream/summary",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d663978-e463-4e29-81e6-31c6c24e980e"
            }
          ]
        },
        {
          "id": "3fec4409-8966-4db6-9818-564c2795154f",
          "name": "hide-a-stream-item",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/activity_stream/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Hide a stream item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c74bcb7-585c-45e3-9a98-d3b4e2f62b1e"
            }
          ]
        },
        {
          "id": "1ceb7301-2f7d-4d66-af9e-2ffe3920af63",
          "name": "list-bookmarks",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/bookmarks",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List bookmarks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9980e963-ac09-4199-a830-11e719f86c8b"
            }
          ]
        }
      ]
    }
  ]
}