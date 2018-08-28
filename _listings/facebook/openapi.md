swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{application}/translations:
    get:
      summary: Get Application Translations
      description: The translated strings for this application.
      operationId: getApplicationTranslations
      x-api-path-slug: applicationtranslations-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Translations
    post:
      summary: Post Application Translations
      description: Uploads translated strings for this application.
      operationId: postApplicationTranslations
      x-api-path-slug: applicationtranslations-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: native_strings
        description: A JSON-encoded array of strings to translate
      responses:
        200:
          description: OK
      tags:
      - Application
      - Translations
    delete:
      summary: Delete Application Translations
      description: Deletes a translation string for this application.
      operationId: deleteApplicationTranslations
      x-api-path-slug: applicationtranslations-delete
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: native_hashes
        description: An array of native hashes
      responses:
        200:
          description: OK
      tags:
      - Application
      - Translations