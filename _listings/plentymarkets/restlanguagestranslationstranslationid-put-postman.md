{
  "info": {
    "name": "Plentymarkets Update a translation",
    "_postman_id": "7703511d-1dcc-41c5-ac4b-e07cb0825ed6",
    "description": "Updates a translation. The ID of the translation must be specified",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "New",
      "item": [
        {
          "id": "cbc08e2a-23ab-41fa-a89c-b8072473eb35",
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
              "id": "e66d9fb3-b69b-4513-b59a-24f04b8d6735"
            }
          ]
        }
      ]
    },
    {
      "name": "Translation",
      "item": [
        {
          "id": "87c12d15-e7ad-49a7-b4de-b6a43410ab33",
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
              "id": "a65c8331-7be0-40fd-b0f5-3c640209528a"
            }
          ]
        },
        {
          "id": "e19c0f74-4f48-4294-a40d-c5e776656dab",
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
              "id": "85ce2338-d866-4a62-a619-7a86f3195f87"
            }
          ]
        },
        {
          "id": "0a49ae3e-9396-4d72-9104-9b24b1d3cede",
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
              "id": "906958a3-1001-45bb-8a5d-8a38021ab4cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "c1424834-bafd-471d-ba1e-65865e822a46",
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
              "id": "7edc0b01-47fc-402d-a285-73ab2616ae69"
            }
          ]
        }
      ]
    }
  ]
}