---
swagger: "2.0"
info:
  title: Search - Tensorflow
  description: Searching for Tensorflow
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
      summary: Search for Tensorflow
      description: Searching Reddit for Tensorflow
      operationId: search
      parameters:
      - in: query
        name: q
        description: The query.
        type: string
        default: Tensorflow
      responses:
        200:
          description: OK
      tags:
      - Search
---
