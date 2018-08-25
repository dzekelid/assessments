---
swagger: "2.0"
x-collection-name: Datumbox
x-complete: 1
info:
  title: DatumBox
  description: datumbox-offers-a-machine-learning-platform-composed-of-14-classifiers-and-natural-language-processing-functions--functions-include-sentiment-analysis-topic-classification-readability-assessment-language-detection-and-much-more-
  version: 1.0.0
host: api.datumbox.com
basePath: 1.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ReadabilityAssessment.json:
    post:
      summary: Evaluates the Readability of the Document
      description: The Readability Assessment function determines the degree of readability
        of a document based on its terms and idioms. The texts are classified as basic,
        intermediate and advanced depending their difficulty.
      operationId: ReadabilityAssessment
      x-api-path-slug: readabilityassessment-json-post
      parameters:
      - in: formData
        name: text
        description: The text that you want to analyze
      responses:
        200:
          description: OK
      tags:
      - Readability
      - Assessment
---