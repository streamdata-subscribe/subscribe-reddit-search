---
swagger: "2.0"
info:
  title: Search - Kafka
  description: Searching for Kafka
  version: 1.0.0
x-collection-name: Reddit  
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search.json:
    get:
      summary: Search for Kafka
      description: Searching Reddit for Kafka
      operationId: search
      parameters:
      - in: query
        name: q
        description: The query.
        type: string
        default: Apache Kafka
      responses:
        200:
          description: OK
      tags:
      - Search
---
