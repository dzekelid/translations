{
  "info": {
    "name": "Plentymarkets Delete multiple translation",
    "_postman_id": "aa04123e-32ef-4806-83b2-dc2804edf05a",
    "description": "Deletes multiple translation. The pluginSetId and languageCode must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Multiple",
      "item": [
        {
          "id": "ed20f4cc-d171-466b-bc58-95297ea6fee2",
          "name": "deleteRestFeedbacksDeleteFeedbacksFeedbacks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/feedbacks/delete_feedbacks/:feedbackIds"
              ],
              "variable": [
                {
                  "id": "feedbackIds",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes multiple feedbacks. A list with IDs of feedbacks must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae92532e-54d8-4a59-9786-4c8d0cb1f241"
            }
          ]
        },
        {
          "id": "a0fa22bb-9f38-4d72-8d42-80cd0e49164b",
          "name": "postRestMarketsSettingsCorrelationsBulk",
          "request": {
            "url": "http://example.com/rest/markets/settings/correlations/bulk",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Creates multiple correlations. The type, market settings ID and the correlation ID for each param combination must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4d9ca48-a5d7-47b2-bb18-4e10b77746df"
            }
          ]
        },
        {
          "id": "47e34166-a468-45e8-8f00-78970afa8e84",
          "name": "deleteRestPluginSetsPluginsetLanguagesLanguagecode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/plugin_sets/:pluginSetId/languages/:languageCode"
              ],
              "query": [
                {
                  "key": "$languageCode",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$pluginSetId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "languageCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "pluginSetId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes multiple translation. The pluginSetId and languageCode must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6924589b-f914-41f9-9469-e53fab99af3e"
            }
          ]
        }
      ]
    },
    {
      "name": "Visibility",
      "item": [
        {
          "id": "fa3736b5-2a6f-425c-8fe7-8be785146e1a",
          "name": "putRestFeedbacksFeedbacksVisibility",
          "request": {
            "url": "http://example.com/rest/feedbacks/feedbacks_visibility?feedbackIds=%7B%7D&isVisible=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Updates the visibility of multiple feedbacks. A list with IDs of feedbacks must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd93fad5-b942-4d55-a728-6d150e65253e"
            }
          ]
        }
      ]
    }
  ]
}