---
name: Google Tag Manager
x-slug: google-tag-manager
description: Deploy and update measurement tags on your websites and mobile apps without
  major code changes and app releases. Use Google Tag Manager to manage tags (such
  as tracking and marketing optimization JavaScript tags) on your site. Without editing
  your site code, you use GTM user interface to add and update AdWords, Google Analytics,
  Floodlight, and non-Google tags. This reduces errors and allows you to to deploy
  tags on your site quickly.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Versions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Google Tag Manager API Get Container Versions
  x-api-slug: google-tag-manager-api
  description: Lists all Container Versions of a GTM Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversions-get-openapi.md
- name: Google Tag Manager API Create Container Version
  x-api-slug: google-tag-manager-api
  description: Creates a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions
  tags: Containers,Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversions-post-openapi.md
- name: Google Tag Manager API Delete Container Version
  x-api-slug: google-tag-manager-api
  description: Deletes a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-delete-openapi.md
- name: Google Tag Manager API Get Container Version
  x-api-slug: google-tag-manager-api
  description: Gets a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-get-openapi.md
- name: Google Tag Manager API Update Container Version
  x-api-slug: google-tag-manager-api
  description: Updates a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}
  tags: Containers,Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-put-openapi.md
- name: Google Tag Manager API Publish Container Version
  x-api-slug: google-tag-manager-api
  description: Publishes a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/publish
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidpublish-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidpublish-post-openapi.md
- name: Google Tag Manager API Restore Container Version
  x-api-slug: google-tag-manager-api
  description: Restores a Container Version. This will overwrite the container's current
    configuration (including its variables, triggers and tags). The operation will
    not have any effect on the version that is being served (i.e. the published version).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/restore
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidrestore-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidrestore-post-openapi.md
- name: Google Tag Manager API Undelete Container Version
  x-api-slug: google-tag-manager-api
  description: Undeletes a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/undelete
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidundelete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidundelete-post-openapi.md
- name: Google Tag Manager API
  x-api-slug: google-tag-manager-api
  description: Deploy and update measurement tags on your websites and mobile apps
    without major code changes and app releases. Use Google Tag Manager to manage
    tags (such as tracking and marketing optimization JavaScript tags) on your site.
    Without editing your site code, you use GTM user interface to add and update AdWords,
    Google Analytics, Floodlight, and non-Google tags. This reduces errors and allows
    you to to deploy tags on your site quickly.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1
  tags: Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/openapi.md
x-common:
- type: x-authentication
  url: https://developers.google.com/tag-manager/api/v1/authorization
- type: x-change-log
  url: https://developers.google.com/tag-manager/api/v1/changelog
- type: x-code
  url: https://developers.google.com/tag-manager/api/v1/libraries
- type: x-documentation
  url: https://developers.google.com/tag-manager/api/v1/
- type: x-performance
  url: https://developers.google.com/tag-manager/api/v1/performance
- type: x-website
  url: https://developers.google.com/tag-manager/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---