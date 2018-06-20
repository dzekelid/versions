---
name: Box
x-slug: box
description: Box is changing how you manage content across your business from simple
  file sharing to building custom apps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
x-kinRank: "9"
x-alexaRank: "443"
tags: Versions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/box/apis.md
specificationVersion: "0.14"
apis:
- name: Box View Versions
  x-api-slug: box
  description: If there are previous versions of this file, this method can be used
    to retrieve information about the older versions. (Versions are only tracked for
    Box users with premium accounts.)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/versions
  tags: Documents,Files, File, , Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/box/filesfile-idversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/box/filesfile-idversions-get-openapi.md
- name: Box Promote Version
  x-api-slug: box
  description: If there are previous versions of this file, this method can be used
    to promote one of the older versions to the top of the stack. This actually mints
    a copy of the old version and puts it on the top of the versions stack. The file
    will have the exact same contents, the same SHA1/etag, and the same name as the
    original. Other properties such as comments do not get updated to their former
    values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/versions/current
  tags: Documents,Files, File, , Versions, Current
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/box/filesfile-idversionscurrent-post-openapi.md
- name: Box Delete Old Version
  x-api-slug: box
  description: Discards a specific file version to the trash. (Depending on the enterprise
    settings for this user, the item will either be actually deleted from Box or moved
    to the trash.)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//files/{FILE_ID}/versions/{VERSION_ID}
  tags: Documents,Files, File, , Versions, Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/box/filesfile-idversionsversion-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/box/filesfile-idversionsversion-id-delete-openapi.md
- name: Box
  x-api-slug: box
  description: Box.net provides a sophisticated API for their online document sharing
    and collaboration web application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/versions/master/_listings/box/openapi.md
x-common:
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-crunchbase
  url: https://crunchbase.com/organization/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/boxdotnet
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-twitter
  url: https://twitter.com/BoxHQ
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---