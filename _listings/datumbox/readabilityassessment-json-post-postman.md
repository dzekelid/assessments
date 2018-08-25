{
  "info": {
    "name": "Datumbox Evaluates the Readability of the Document",
    "_postman_id": "4f0f1b56-a6ac-4fe4-9572-c2024517eb93",
    "description": "The Readability Assessment function determines the degree of readability of a document based on its terms and idioms. The texts are classified as basic, intermediate and advanced depending their difficulty.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Adult Content",
      "item": [
        {
          "id": "61cfc47a-3fc1-47fa-a052-25b3e1d1fd02",
          "name": "AdultContentDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/AdultContentDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Adult Content Detection function classifies the documents as adult or noadult based on their context. It can be used to detect whether a document contains content unsuitable for minors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e89ba42-1a4c-4972-b1df-8822b7fb3edf"
            }
          ]
        }
      ]
    },
    {
      "name": "Commercial",
      "item": [
        {
          "id": "9dcdc7c2-d53d-4a68-a9b3-795a088ed8d9",
          "name": "CommercialDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/CommercialDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Commercial Detection function labels the documents as commercial or non-commercial based on their keywords and expressions. It can be used to detect whether a website is commercial or not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a68ed487-46cf-45ec-b91f-f921396cd681"
            }
          ]
        }
      ]
    },
    {
      "name": "DocumentsSimilarity",
      "item": [
        {
          "id": "9ba9c68a-865e-455e-ac75-e49b5b4918a3",
          "name": "DocumentSimilarity",
          "request": {
            "url": "http://api.datumbox.com/1.0/DocumentSimilarity.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "copy",
                  "value": "{}",
                  "disabled": false,
                  "description": "The second text"
                },
                {
                  "key": "original",
                  "value": "{}",
                  "disabled": false,
                  "description": "The first text"
                }
              ]
            },
            "description": "The Document Similarity function estimates the degree of similarity between two documents. It can be used to detect duplicate webpages or detect plagiarism."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4b07b09-c6a3-4d17-9503-41129f062f33"
            }
          ]
        }
      ]
    },
    {
      "name": "Educational",
      "item": [
        {
          "id": "380580e7-5ded-4153-afa2-26a913050706",
          "name": "EducationalDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/EducationalDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Educational Detection function classifies the documents as educational or non-educational based on their context. It can be used to detect whether a website is educational or not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1631693-dbc8-474d-a541-e3bc346d9335"
            }
          ]
        }
      ]
    },
    {
      "name": "Gender",
      "item": [
        {
          "id": "d04c2ccd-a933-45c0-8e91-331cd06a972c",
          "name": "GenderDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/GenderDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Gender Detection function identifies if a particular document is written-by or targets-to a man or a woman based on the context, the words and the idioms found in the text."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "feb5089d-6ac3-4a1a-af99-e6a3a2eb9fb3"
            }
          ]
        }
      ]
    },
    {
      "name": "Keyword",
      "item": [
        {
          "id": "fed55a85-0d83-475d-8a44-5128ad2d1389",
          "name": "KeywordExtraction",
          "request": {
            "url": "http://api.datumbox.com/1.0/KeywordExtraction.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "n",
                  "value": "{}",
                  "disabled": false,
                  "description": "The number of keyword combinations (n-grams) that you wish to extract"
                },
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Keyword Extraction function enables you to extract from an arbitrary document all the keywords and word-combinations along with their occurrences in the text."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "212c6682-f3cc-40d8-a46c-24ca28c98493"
            }
          ]
        }
      ]
    },
    {
      "name": "Language",
      "item": [
        {
          "id": "01295def-9bce-4269-8979-2e557b62e91b",
          "name": "LanguageDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/LanguageDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Language Detection function identifies the natural language of the given document based on its words and context. This classifier is able to detect 96 different languages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "450d4153-d4eb-4a7d-b11b-a88ea9ef8377"
            }
          ]
        }
      ]
    },
    {
      "name": "Readability",
      "item": [
        {
          "id": "c471a6bd-493d-48fc-90fe-fb87cb7fcee1",
          "name": "ReadabilityAssessment",
          "request": {
            "url": "http://api.datumbox.com/1.0/ReadabilityAssessment.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Readability Assessment function determines the degree of readability of a document based on its terms and idioms. The texts are classified as basic, intermediate and advanced depending their difficulty."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f79bc4d9-5a10-4486-bf6c-52e1a570f3c0"
            }
          ]
        }
      ]
    }
  ]
}