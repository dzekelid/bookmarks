{
  "info": {
    "name": "Instructure Canvas Users API Create bookmark",
    "_postman_id": "fa1a2e8b-9562-4be5-b01b-6916bd2b03d0",
    "description": "Create bookmark.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "1e42db18-9506-4a2b-85a7-28bd77f495de",
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
              "id": "fc05adf6-7cbb-4262-b4be-dfb4839ac780"
            }
          ]
        },
        {
          "id": "593fa8cf-cbd9-43a3-a61c-6214df4c2458",
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
              "id": "165da4a7-5f0d-4ba7-9f9c-7c0485d38cd1"
            }
          ]
        },
        {
          "id": "a9c3c687-46c9-41c5-b032-2e772b4bcc54",
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
              "id": "810f3556-c346-4871-9528-d9320e9cb250"
            }
          ]
        },
        {
          "id": "1645d338-dee7-4d43-ab88-072564a8c5b3",
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
              "id": "626a901a-c457-40d7-92c7-6c7643fa4dd8"
            }
          ]
        },
        {
          "id": "c2be6af8-08a3-4a85-b622-c7f4b3315fe9",
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
              "id": "0a29688b-5031-4ff3-aecd-0f3751a402de"
            }
          ]
        },
        {
          "id": "9e4a04d9-ae67-4f95-9ff6-e40732243f64",
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
              "id": "8eca9d7b-ebe0-41cc-b57f-78e872069839"
            }
          ]
        },
        {
          "id": "e27e0262-8e4f-4ee2-b186-e67a1324517f",
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
              "id": "c25d37d6-6d99-4794-a820-334384bd07ac"
            }
          ]
        }
      ]
    }
  ]
}