---
swagger: "2.0"
info:
  title: Answers - Kubernetes
  description: Subscribe to Stack Overflow answers for Kubernetes.
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
  /answers:
    get:
      summary: Get Answers for Kubernetes
      description: Returns answers for Stack Overflow
      operationId: subscribeAnswers
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
        default: Kubernetes
      tags:
      - Answers
---
