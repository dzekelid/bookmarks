{
  "info": {
    "name": "Instructure Canvas Users API Get bookmark",
    "_postman_id": "1d5032d1-8cdb-4cd4-9c20-ded8728658cd",
    "description": "Get bookmark.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "75cb65b7-d221-470a-9676-7b22b488ba62",
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
              "id": "f3e47655-4d3c-41aa-a77a-b799a18de4b6"
            }
          ]
        },
        {
          "id": "ff6456b5-07ce-4424-9da2-b9492a25415b",
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
              "id": "7c4ac915-e88c-45b6-96ec-eaf4529863a0"
            }
          ]
        },
        {
          "id": "71ff77a4-54a4-4c1e-9242-b4549df20cdc",
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
              "id": "606006b9-e62a-49aa-a286-dfe425bdf536"
            }
          ]
        },
        {
          "id": "7f3b3efd-e7c4-4db1-8720-0754ecbce86e",
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
              "id": "35e66f96-9092-43cf-9ae4-3f157dd8d0c7"
            }
          ]
        },
        {
          "id": "c7416c6f-c4a1-486c-a254-9f10a6606ae2",
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
              "id": "6e6385aa-f0ef-44f2-bcda-4d1c25292975"
            }
          ]
        },
        {
          "id": "b8e23e76-d083-4e81-a4bf-568899d823b0",
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
              "id": "dccdc094-5a41-45df-bcef-a3c8afd0530b"
            }
          ]
        },
        {
          "id": "24541e4b-605a-44c9-bf8c-ff7a9bf7dcef",
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
              "id": "6669bd62-972e-4e5f-bbf0-a16660d7c844"
            }
          ]
        },
        {
          "id": "eaee07e3-a746-42f6-9c1f-520c5f34ca5e",
          "name": "get-bookmark",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1114e606-1f30-4b6a-823d-0682db23e3ca"
            }
          ]
        },
        {
          "id": "276d3187-17aa-446b-bc23-65cc68c68c71",
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
              "id": "579645ac-8d66-411c-98ec-83e153453087"
            }
          ]
        }
      ]
    }
  ]
}