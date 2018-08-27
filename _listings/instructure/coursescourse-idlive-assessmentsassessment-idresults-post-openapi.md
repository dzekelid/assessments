---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Create live assessment results
  description: Create live assessment results.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/live_assessments:
    get:
      summary: List live assessments
      description: List live assessments.
      operationId: list-live-assessments
      x-api-path-slug: coursescourse-idlive-assessments-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Live
      - Assessments
    post:
      summary: Create or find a live assessment
      description: Create or find a live assessment.
      operationId: create-or-find-a-live-assessment
      x-api-path-slug: coursescourse-idlive-assessments-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Live
      - Assessments
  /courses/{course_id}/live_assessments/assessment_id/results:
    get:
      summary: List live assessment results
      description: List live assessment results.
      operationId: list-live-assessment-results
      x-api-path-slug: coursescourse-idlive-assessmentsassessment-idresults-get
      parameters:
      - in: query
        name: user_id
        description: If set, restrict results to those for this user
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Live
      - Assessments
      - Assessment
      - Id
      - Results
    post:
      summary: Create live assessment results
      description: Create live assessment results.
      operationId: create-live-assessment-results
      x-api-path-slug: coursescourse-idlive-assessmentsassessment-idresults-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Live
      - Assessments
      - Assessment
      - Id
      - Results
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