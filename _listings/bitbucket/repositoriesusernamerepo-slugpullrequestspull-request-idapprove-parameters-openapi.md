---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Pullrequests Pull Request  Approve
  description: Parameters repositories username repo slug pullrequests pull request  approve
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
    put:
      summary: Update Repositories Username Repo Slug Pullrequests Pull Request
      description: |-
        Mutates the specified pull request.

        This can be used to change the pull request's branches or description.

        Only open pull requests can be mutated.
      operationId: putRepositoriesUsernameRepoSlugPullrequestsPullRequest
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-id-put
      parameters:
      - in: path
        name: pull_request_id
        description: The id of the open pull request
      - in: path
        name: repo_slug
        description: 'This can either be the repository slug or the UUID of the repository,surrounded
          by curly-braces, for example: `{repository UUID}`'
      - in: path
        name: username
        description: 'This can either be the username or the UUID of the user,surrounded
          by curly-braces, for example: `{user UUID}`'
      - in: body
        name: _body
        description: The pull request that is to be updated
        schema:
          $ref: '#/definitions/holder'
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
  /repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/activity:
    get:
      summary: Get Repositories Username Repo Slug Pullrequests Pull Request  Activity
      description: |-
        Returns a paginated list of the pull request's activity log.

        This includes comments that were made by the reviewers, updates and
        approvals.
      operationId: getRepositoriesUsernameRepoSlugPullrequestsPullRequestActivity
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idactivity-get
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
        description: 'This can either be the username or the UUID of the user,surrounded
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
      - ""
      - Activity
    parameters:
      summary: Parameters Repositories Username Repo Slug Pullrequests Pull Request  Activity
      description: Parameters repositories username repo slug pullrequests pull request  activity
      operationId: parametersRepositoriesUsernameRepoSlugPullrequestsPullRequestActivity
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idactivity-parameters
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
      - ""
      - Activity
  /repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/approve:
    delete:
      summary: Delete Repositories Username Repo Slug Pullrequests Pull Request  Approve
      description: Delete repositories username repo slug pullrequests pull request  approve
      operationId: deleteRepositoriesUsernameRepoSlugPullrequestsPullRequestApprove
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idapprove-delete
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
      - ""
      - Approve
    parameters:
      summary: Parameters Repositories Username Repo Slug Pullrequests Pull Request  Approve
      description: Parameters repositories username repo slug pullrequests pull request  approve
      operationId: parametersRepositoriesUsernameRepoSlugPullrequestsPullRequestApprove
      x-api-path-slug: repositoriesusernamerepo-slugpullrequestspull-request-idapprove-parameters
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
      - ""
      - Approve
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