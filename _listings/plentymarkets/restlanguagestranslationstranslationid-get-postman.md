{
  "info": {
    "name": "Plentymarkets Get a translation",
    "_postman_id": "be9e12fa-fdbd-49ff-976b-f53b989af2e3",
    "description": "Gets a translation. The ID of the translation must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "New",
      "item": [
        {
          "id": "d5ca393f-3b5d-4a54-a822-477a4a1e7871",
          "name": "postRestLanguagesTranslations",
          "request": {
            "url": "http://example.com/rest/languages/translations?$fileName=%7B%7D&$key=%7B%7D&$languageCode=%7B%7D&$pluginName=%7B%7D&$pluginSetId=%7B%7D&$value=%7B%7D",
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
            "description": "Creates a new translation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8feb7b0c-5d2d-4e81-8502-336542ef1441"
            }
          ]
        }
      ]
    },
    {
      "name": "Translation",
      "item": [
        {
          "id": "bb0daf45-ab33-4126-b728-34b491823efe",
          "name": "getRestLanguagesTranslationsTranslation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/languages/translations/:translationId"
              ],
              "query": [
                {
                  "key": "$id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "translationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
            "description": "Gets a translation. The ID of the translation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf659b8f-97df-466d-bd77-4b18c0de9b3e"
            }
          ]
        },
        {
          "id": "deb1f48e-2e0b-4f91-8622-2a6e576368de",
          "name": "putRestLanguagesTranslationsTranslation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/languages/translations/:translationId"
              ],
              "query": [
                {
                  "key": "$fileName",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$languageCode",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$pluginName",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$pluginSetId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "translationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Updates a translation. The ID of the translation must be specified"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdd23df1-11cd-4cc4-9d28-58c600bedcfd"
            }
          ]
        },
        {
          "id": "eeaa5eaf-45b2-4749-95e0-ffc866c27a52",
          "name": "deleteRestLanguagesTranslationsTranslation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/languages/translations/:translationId"
              ],
              "query": [
                {
                  "key": "$translationId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "translationId",
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
            "description": "Deletes a translation. The ID of the translation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "049b04a3-d933-401a-9bf2-81e5d03f31a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "99b0bf99-013f-4a14-bcb8-4adc77a70c93",
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
              "id": "acb9b30a-e4ba-4869-9acc-9d87ac5c8659"
            }
          ]
        }
      ]
    }
  ]
}