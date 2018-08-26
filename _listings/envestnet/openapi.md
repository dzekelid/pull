---
swagger: "2.0"
x-collection-name: Envestnet
x-complete: 1
info:
  title: Crunch Base
  description: the-crunchbase-api-is-a-relatively-straightforward-rest-service-that-allows-developers-to-access-data-in-the-business-graph-
  termsOfService: https://data.crunchbase.com/v3/page/accessing-the-dataset
  contact:
    name: Crunchbase
    url: https://groups.google.com/forum/#!forum/crunchbase-api
    email: data@crunchbase.com
  version: v3
host: api.crunchbase.com
basePath: /v/3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /acquisitions/{uuid}:
    get:
      summary: Acquistions
      description: Pull from Acquisition
      operationId: acquistions
      x-api-path-slug: acquisitionsuuid-get
      parameters:
      - in: query
        name: user_key
        description: This user_key is used to validate each developers access to the
          API and ensure that any rate limits or quotas are respected
      - in: path
        name: uuid
        description: The UUID of the acquisition
      responses:
        200:
          description: OK
      tags:
      - Acquisitions
      - Uuid
---