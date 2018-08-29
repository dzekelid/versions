swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 1
info:
  title: Bitbucket
  description: code-against-the-bitbucket-api-to-automate-simple-tasks-embed-bitbucket-data-into-your-own-site-build-mobile-or-desktop-apps-or-even-add-custom-ui-addons-into-bitbucket-itself-using-the-connect-framework-
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
  /repositories/{username}/{repo_slug}/versions:
    get:
      summary: Get Repositories Username Repo Slug Versions
      description: |-
        Returns the versions that have been defined in the issue tracker.

        This resource is only available on repositories that have the issue
        tracker enabled.
      operationId: getRepositoriesUsernameRepoSlugVersions
      x-api-path-slug: repositoriesusernamerepo-slugversions-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Versions
    parameters:
      summary: Parameters Repositories Username Repo Slug Versions
      description: Parameters repositories username repo slug versions
      operationId: parametersRepositoriesUsernameRepoSlugVersions
      x-api-path-slug: repositoriesusernamerepo-slugversions-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Versions
  /repositories/{username}/{repo_slug}/versions/{version_id}:
    get:
      summary: Get Repositories Username Repo Slug Versions Version
      description: Get repositories username repo slug versions version
      operationId: getRepositoriesUsernameRepoSlugVersionsVersion
      x-api-path-slug: repositoriesusernamerepo-slugversionsversion-id-get
      parameters:
      - in: path
        name: version_id
        description: The versions id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Versions
      - Version
    parameters:
      summary: Parameters Repositories Username Repo Slug Versions Version
      description: Parameters repositories username repo slug versions version
      operationId: parametersRepositoriesUsernameRepoSlugVersionsVersion
      x-api-path-slug: repositoriesusernamerepo-slugversionsversion-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Versions
      - Version