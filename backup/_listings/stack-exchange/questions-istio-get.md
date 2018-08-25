---
swagger: "2.0"
info:
  title: Questions - Istio
  description: Subscribe to Stack Overflow questions for Istio.
  version: "2.0"
host: api.stackexchange.com
x-collection-name: Stack Exchange
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /questions:
    get:
      summary: Get Questions for Istio
      description: Subscribe to questions from Stack Overflow.
      operationId: getQuestions
      parameters:
      - in: query
        name: order
        default: desc
      - in: query
        name: site
        description: The site to return results for.
        default: stackoverflow
      - in: query
        name: sort
        default: activity
      - in: query
        name: tagged
        description: The tag to return.
        default: Istio
      tags:
      - Questions
---
