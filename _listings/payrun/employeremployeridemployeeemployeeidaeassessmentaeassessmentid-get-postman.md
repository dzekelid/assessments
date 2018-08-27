{
  "info": {
    "name": "Pay Run.IO Get the auto enrolment assessment",
    "_postman_id": "5e512bfa-967d-4688-bde3-a2c9cf0ba299",
    "description": "Gets the auto enrolment assessment from the specified employee",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "DPMessage",
      "item": [
        {
          "id": "80379da3-e631-442d-b2b8-082f27e46c00",
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
              "id": "4ba60146-d0fc-417d-a2f6-694a89d00994"
            }
          ]
        },
        {
          "id": "d04d6d76-f2b9-4c87-8e18-bb7a81e6759f",
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
              "id": "5ee29797-d92f-4217-8d3e-38feb2284e5a"
            }
          ]
        }
      ]
    },
    {
      "name": "Patches",
      "item": [
        {
          "id": "fc62d75e-ba46-4fe5-bf75-fd154f4ea491",
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
              "id": "bc78d730-437d-41ff-8bd8-e98211a1a69a"
            }
          ]
        }
      ]
    },
    {
      "name": "DPMessages",
      "item": [
        {
          "id": "fa73224a-e2f4-4104-b295-a94e256fc7b7",
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
              "id": "ff142d64-abcd-4134-8cca-6947af4eb0b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto",
      "item": [
        {
          "id": "71507d4d-4a08-41cd-88a4-1dcd901105c3",
          "name": "GetAEAssessmentFromEmployee",
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
            "description": "Gets the auto enrolment assessment from the specified employee"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "878a0ba8-2946-44b3-a0f5-5a7b857cda5a"
            }
          ]
        },
        {
          "id": "0265f668-a567-4fe1-ac57-cc848f9415a1",
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
              "id": "67b39c9f-8c54-42ca-8dc6-d31e7ade611a"
            }
          ]
        }
      ]
    }
  ]
}