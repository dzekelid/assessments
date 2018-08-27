---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Get the auto enrolment assessments
  description: Gets all auto enrolment assessments from the specified pay run
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employer/{EmployerId}/Employee/{EmployeeId}/AEAssessments:
    get:
      summary: Get the auto enrolment assessments
      description: Gets all auto enrolment assessments from the specified employee
      operationId: GetAEAssessmentsFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidaeassessments-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Enrolment
      - Assessments
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/AEAssessments:
    get:
      summary: Get the auto enrolment assessments
      description: Gets all auto enrolment assessments from the specified pay run
      operationId: GetAEAssessmentsFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidaeassessments-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Enrolment
      - Assessments
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---