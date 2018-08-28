---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Pullrequests Pull Request
  description: Parameters repositories username repo slug pullrequests pull request
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}:
    get:
      summary: Get Repositories Username Repo Slug Pullrequests Pull Request
      description: Get repositories username repo slug pullrequests pull request
      operationId: getRepositoriesUsernameRepoSlugPullrequestsPullRequest
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-id-get
      parameters:
      - in: path
        name: pull_request_id
        description: The id of the pull request
      - in: path
        name: repo_slug
        description: 'This can either be the repository slug or the UUID of the repository,surrounded
          by curly-braces, for example: `{repository UUID}`'
      - in: path
        name: username
        description: 'This can either be the username or the UUID of the account,surrounded
          by curly-braces, for example: `{user UUID}`'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
    parameters:
      summary: Parameters Repositories Username Repo Slug Pullrequests Pull Request
      description: Parameters repositories username repo slug pullrequests pull request
      operationId: parametersRepositoriesUsernameRepoSlugPullrequestsPullRequest
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pullrequests
      - Pull
      - Request
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