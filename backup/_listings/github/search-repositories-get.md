---
swagger: "2.0"
info:
  title: GitHub
  description: GitHub is the best place to share code with friends, co-workers, classmates,
    and complete strangers. Over 24 million people use GitHub to build amazing things
    together across 67 million repositories. With the collaborative features of GitHub.com
    and GitHub Business, it has never been easier for individuals and teams to write
    faster, better code.
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
x-collection-name: GitHub
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/repositories:
    get:
      summary: Get Search Repositories
      description: Search repositories
      operationId: search-repositories
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: order
        description: The sort field
      - in: query
        name: q
        description: The search terms
      - in: query
        name: sort
        description: If not provided, results are sorted by best match
      responses:
        200:
          description: OK
      tags:
      - search
      - repositories
