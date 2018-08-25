---
swagger: "2.0"
info:
  title: Search - Istio
  description: Searching for Istio
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
      summary: Search for Istio
      description: Searching Reddit for Istio
      operationId: search
      parameters:
      - in: query
        name: q
        description: The query.
        type: string
        default: Istio
      responses:
        200:
          description: OK
      tags:
      - Search
---
