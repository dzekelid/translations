swagger: "2.0"
x-collection-name: Europeana
x-complete: 1
info:
  title: Europeana
  description: this-swagger-api-console-provides-an-overview-of-an-interface-to-the-europeana-rest-api--you-can-build-and-test-anything-from-the-simplest-search-to-a-complex-query-using-facetlist-such-as-dates-geotags-and-permissions--for-more-help-and-information-head-to-our-comprehensive-a-hrefhttplabs-europeana-euapionline-documentationa-
  termsOfService: http://www.europeana.eu/portal/en/rights.html
  contact:
    name: http://labs.europeana.eu/api
  version: 1.0.0
host: www.europeana.eu
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /translateQuery.json:
    get:
      summary: translate a term to different languages
      description: Translate a term to different languages.
      operationId: translateQueryUsingGET
      x-api-path-slug: translatequery-json-get
      parameters:
      - in: query
        name: callback
        description: callback
      - in: query
        name: languageCodes
        description: languageCodes
      - in: query
        name: profile
        description: profile
      - in: query
        name: term
        description: term
      - in: query
        name: wskey
        description: wskey
      responses:
        200:
          description: OK
      tags:
      - Translations
      - Query