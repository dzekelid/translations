{
  "info": {
    "name": "Google Translate API Translate Text",
    "_postman_id": "b590a83c-e9f9-4c65-9404-9e36661a4dd4",
    "description": "Returns text translations from one language to another.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Translate",
      "item": [
        {
          "id": "98efddb5-7bb9-4bf4-aa69-8a7cf597daf9",
          "name": "language.translations.list",
          "request": {
            "url": "http://www.googleapis.com/language/translate/v2?cid=%7B%7D&format=%7B%7D&q=%7B%7D&source=%7B%7D&target=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns text translations from one language to another."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d65a8983-d1da-497c-91c8-6f7e2ff6f1ab"
            }
          ]
        }
      ]
    }
  ]
}