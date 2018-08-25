---
swagger: "2.0"
info:
  title: Search - Kubernetes
  description: Searching for Kubernetes
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
      summary: Search for Kubernetes
      description: Searching Reddit for Kubernetes
      operationId: search
      parameters:
      - in: query
        name: q
        description: The query.
        type: string
        default: Kubernetes
      responses:
        200:
          description: OK
      tags:
      - Search
---
