---
name: Google Tag Manager
description: Deploy and update measurement tags on your websites and mobile apps without
  major code changes and app releases. Use Google Tag Manager to manage tags (such
  as tracking and marketing optimization JavaScript tags) on your site. Without editing
  your site code, you use GTM user interface to add and update AdWords, Google Analytics,
  Floodlight, and non-Google tags. This reduces errors and allows you to to deploy
  tags on your site quickly.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Tags
- Stack Network
- Google APIs
created: "2018-03-24"
modified: "2018-03-24"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google Tag Manager API
  description: Deploy and update measurement tags on your websites and mobile apps
    without major code changes and app releases
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: ""
  baseURL: ://www.googleapis.com//tagmanager/v1
  tags: Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accounts-accountid-containers-containerid-versions-containerversionid-undelete-post.md
- name: Google Tag Manager API Publish Container Version
  description: Publishes a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: http:://www.googleapis.com//tagmanager/v1
  tags: Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accounts-accountid-containers-containerid-versions-containerversionid-publish-post.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/google-tag-manager/accounts-accountid-containers-containerid-versions-containerversionid-publish-post-postman.md
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