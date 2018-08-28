{
  "info": {
    "name": "Plentymarkets Delete a translation",
    "_postman_id": "567bbd39-21eb-41e3-8284-128fe5066136",
    "description": "Deletes a translation. The ID of the translation must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "New",
      "item": [
        {
          "id": "d3ef3ffb-140f-4882-bb90-3a57585d7d83",
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
              "id": "227b4a6d-5f63-4cf2-80f3-68bf33423842"
            }
          ]
        }
      ]
    },
    {
      "name": "Translation",
      "item": [
        {
          "id": "fe4a0ecc-4923-4e01-873c-13cefbb302c3",
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
              "id": "2fe7d17a-fffe-41f3-83af-2e021d39089a"
            }
          ]
        },
        {
          "id": "ca828f90-32fb-4410-85ce-87ac20dd86b4",
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
              "id": "90142c7b-ebed-45c5-8b1e-0997b714e3b8"
            }
          ]
        },
        {
          "id": "0df96b6e-5c81-4b5f-9245-ad4445c349e6",
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
              "id": "f837c863-71cb-4a11-b81a-00c5bc8693a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "dfba01ea-0e43-4303-a091-f8f06185cfa6",
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
              "id": "1b3db761-f727-40b1-84f8-b5f28c769c84"
            }
          ]
        }
      ]
    }
  ]
}