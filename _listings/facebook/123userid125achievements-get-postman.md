{
  "info": {
    "name": "Facebook Get User Achievements",
    "_postman_id": "f07b8d90-700c-4269-8ec9-fe991542c8cd",
    "description": "User Achievements",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "018105e0-5f10-497b-800c-2dea5f5b5847",
          "name": "getUserAchievements",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;user-id&#125;/achievements?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User Achievements"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1db7c5fa-c9d5-40db-bcfa-6cf399b7ebf4"
            }
          ]
        }
      ]
    }
  ]
}