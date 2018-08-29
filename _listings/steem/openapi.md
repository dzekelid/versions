swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_version:
    get:
      summary: get version of Steem
      description: Returns version information of connected Steem node/websocket.
      operationId: returns-version-information-of-connected-steem-nodewebsocket
      x-api-path-slug: get-version-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Version
      - Of
      - Steem
  /get_hardfork_version:
    get:
      summary: get_hardfork_version
      description: get_hardfork_version
      operationId: get-hardfork-version
      x-api-path-slug: get-hardfork-version-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Hardfork
      - Version