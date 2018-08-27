{
  "info": {
    "name": "Facebook Post User Achievements",
    "_postman_id": "a8e3ad3b-d66a-4ef2-b666-60265f13b264",
    "description": "Posts an achievement for the user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Application",
      "item": [
        {
          "id": "021d5149-1264-4143-9bdf-5724cf9afb21",
          "name": "postApplicationAchievements",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/achievements"
              ],
              "query": [
                {
                  "key": "achievement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "display_order",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Registers an achievement for the application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa57646e-71b3-4190-8eb0-0416a4393099"
            }
          ]
        },
        {
          "id": "c4cdc011-3e4f-47c7-818d-7364e69cee05",
          "name": "deleteApplicationAchievements",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":application/achievements"
              ],
              "query": [
                {
                  "key": "achievement",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unregisters an achievement for the application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ca74a96-c465-4ebc-a750-209cd99f5cd9"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "ccafc2cc-5f7e-40bc-9942-0074140ed0e0",
          "name": "postUserAchievements",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.facebook.com",
              "path": [
                ":user/achievements"
              ],
              "query": [
                {
                  "key": "achievement",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts an achievement for the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6db6f26-2bea-4b33-a5da-77429f13fc3f"
            }
          ]
        }
      ]
    }
  ]
}