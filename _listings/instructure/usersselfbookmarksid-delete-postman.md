{
  "info": {
    "name": "Instructure Canvas Users API Delete bookmark",
    "_postman_id": "3daccab4-24cb-46b1-8bf4-c1d7e31d77ca",
    "description": "Delete bookmark.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "fd76eec0-3012-485b-a0d9-9eecbcc95d74",
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
              "id": "48e5dd2b-3006-46cf-ad3b-881cd017c9ba"
            }
          ]
        },
        {
          "id": "2c970d06-6856-4dd7-b789-3884c6085fb1",
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
              "id": "47d6a15e-27bf-4869-b963-1090a0c348da"
            }
          ]
        },
        {
          "id": "a8d9d537-db62-4100-94a3-fcd2311d737a",
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
              "id": "8372abf7-70c1-40eb-98c5-05ada937f28f"
            }
          ]
        },
        {
          "id": "ef3dc310-df94-414e-b5a1-2e9136503f00",
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
              "id": "f0c91bfd-8294-4643-adc5-ad546725ef29"
            }
          ]
        },
        {
          "id": "892930f8-df1c-4487-8046-c7104ed70406",
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
              "id": "8473c8a2-06e1-4433-8463-2fca1f6fda79"
            }
          ]
        },
        {
          "id": "6fd0c786-b9ae-4401-a9bd-775d7e11d149",
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
              "id": "be77faa2-38c3-4603-898d-534f5cc5ae47"
            }
          ]
        },
        {
          "id": "92672aae-50ff-47cc-8a2d-ed9cadb2c832",
          "name": "create-bookmark",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/bookmarks?data=%7B%7D&name=%7B%7D&position=%7B%7D&url=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae4a5fee-8d6d-494a-b672-0b0dcd55396c"
            }
          ]
        },
        {
          "id": "a6e5d4ca-9d11-4b70-8f9f-1630c448d8ef",
          "name": "delete-bookmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/bookmarks/:id"
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
            "description": "Delete bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1e2a896-0cec-49b7-a4a4-076219f08da7"
            }
          ]
        }
      ]
    }
  ]
}