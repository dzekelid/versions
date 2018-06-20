---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Versions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket Get Repositories Username Repo Slug Versions
  x-api-slug: bitbucket
  description: |-
    Returns the versions that have been defined in the issue tracker.

    This resource is only available on repositories that have the issue
    tracker enabled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/versions
  tags: Repositories, Username, Repo, Slug, Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/repositoriesusernamerepo-slugversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/repositoriesusernamerepo-slugversions-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Versions
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug versions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/versions
  tags: Repositories, Username, Repo, Slug, Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/repositoriesusernamerepo-slugversions-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/repositoriesusernamerepo-slugversions-parameters-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Versions Version
  x-api-slug: bitbucket
  description: Get repositories username repo slug versions version
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/versions/{version_id}
  tags: Repositories, Username, Repo, Slug, Versions, Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/repositoriesusernamerepo-slugversionsversion-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/repositoriesusernamerepo-slugversionsversion-id-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Versions Version
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug versions version
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/versions/{version_id}
  tags: Repositories, Username, Repo, Slug, Versions, Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/repositoriesusernamerepo-slugversionsversion-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/repositoriesusernamerepo-slugversionsversion-id-parameters-openapi.md
- name: Bitbucket
  x-api-slug: bitbucket
  description: Collaborate on code with inline comments and pull requests. Manage
    and share your Git repositories to build and ship software, as a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/bitbucket/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---