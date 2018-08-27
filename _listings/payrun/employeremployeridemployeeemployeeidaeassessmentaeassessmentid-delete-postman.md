{
  "info": {
    "name": "Pay Run.IO Delete auto enrolment assessment",
    "_postman_id": "0319dcc8-8298-4eac-8829-5ee45b030024",
    "description": "Deletes an existing auto enrolment assessment for the employee. Used to remove historical assessments",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "DPMessage",
      "item": [
        {
          "id": "ca06d7c2-7e38-4b97-a4ee-7172f8d89e54",
          "name": "GetDpsMessageFromEmployer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/DpsMessage/:DpsMessageId"
              ],
              "variable": [
                {
                  "id": "DpsMessageId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the DPS message"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df7a5d90-5f73-45ce-9242-af60e98b3f46"
            }
          ]
        },
        {
          "id": "3b5b5d50-c96a-434d-aed4-db8e395ab2c5",
          "name": "DeleteDpsMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/DpsMessage/:DpsMessageId"
              ],
              "variable": [
                {
                  "id": "DpsMessageId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the DPS message"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85a957bc-d7ca-4162-b0a2-e3f891778681"
            }
          ]
        }
      ]
    },
    {
      "name": "Patches",
      "item": [
        {
          "id": "d7c1d0ef-d64a-4d55-880d-fb0676f9d97e",
          "name": "PatchDpsMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/DpsMessage/:DpsMessageId"
              ],
              "variable": [
                {
                  "id": "DpsMessageId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Patches the specified DPS message with the supplied values"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0d56d22-0929-4f73-84e3-1dcb8f356f38"
            }
          ]
        }
      ]
    },
    {
      "name": "DPMessages",
      "item": [
        {
          "id": "c737af29-b177-4530-8e5d-6e5ebce12372",
          "name": "GetDpsMessagesFromEmployer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/DpsMessages"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the DPS message links"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd3b37d0-9514-4cf6-af38-6303d7f566aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto",
      "item": [
        {
          "id": "455ae991-877d-4081-9feb-a82cd3287ad3",
          "name": "DeleteAEAssessment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employee/:EmployeeId/AEAssessment/:AEAssessmentId"
              ],
              "variable": [
                {
                  "id": "AEAssessmentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing auto enrolment assessment for the employee. Used to remove historical assessments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79dacc19-9444-426f-9cc1-f15228e481af"
            }
          ]
        }
      ]
    }
  ]
}