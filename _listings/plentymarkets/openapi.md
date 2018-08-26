---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/languages/translations:
    post:
      summary: Create a new translation
      description: Creates a new translation.
      operationId: postRestLanguagesTranslations
      x-api-path-slug: restlanguagestranslations-post
      parameters:
      - in: query
        name: $fileName
        description: The of the file
      - in: query
        name: $key
        description: The translation key
      - in: query
        name: $languageCode
        description: The language code for the translation
      - in: query
        name: $pluginName
        description: The name of the plugin
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: query
        name: $value
        description: The value of the translation
      responses:
        200:
          description: OK
      tags:
      - New
      - Translation
  /rest/languages/translations/{translationId}:
    delete:
      summary: Delete a translation
      description: Deletes a translation. The ID of the translation must be specified.
      operationId: deleteRestLanguagesTranslationsTranslation
      x-api-path-slug: restlanguagestranslationstranslationid-delete
      parameters:
      - in: query
        name: $translationId
        description: The ID of the translation
      - in: path
        name: translationId
      responses:
        200:
          description: OK
      tags:
      - Translation
    get:
      summary: Get a translation
      description: Gets a translation. The ID of the translation must be specified.
      operationId: getRestLanguagesTranslationsTranslation
      x-api-path-slug: restlanguagestranslationstranslationid-get
      parameters:
      - in: query
        name: $id
        description: The ID of the translation
      - in: path
        name: translationId
      responses:
        200:
          description: OK
      tags:
      - Translation
    put:
      summary: Update a translation
      description: Updates a translation. The ID of the translation must be specified
      operationId: putRestLanguagesTranslationsTranslation
      x-api-path-slug: restlanguagestranslationstranslationid-put
      parameters:
      - in: query
        name: $fileName
        description: The value of the translation
      - in: query
        name: $id
        description: The ID of the translation
      - in: query
        name: $key
        description: The translation key
      - in: query
        name: $languageCode
        description: The language code for the translation
      - in: query
        name: $pluginName
        description: The name of the plugin
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: query
        name: $value
        description: The value of the translation
      - in: path
        name: translationId
      responses:
        200:
          description: OK
      tags:
      - Translation
  /rest/plugin_sets/{pluginSetId}/languages/{languageCode}:
    delete:
      summary: Delete multiple translation
      description: Deletes multiple translation. The pluginSetId and languageCode
        must be specified.
      operationId: deleteRestPluginSetsPluginsetLanguagesLanguagecode
      x-api-path-slug: restplugin-setspluginsetidlanguageslanguagecode-delete
      parameters:
      - in: query
        name: $languageCode
        description: The code of the language
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: path
        name: languageCode
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Translation
---