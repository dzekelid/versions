swagger: "2.0"
x-collection-name: Google Cloud Key Management Service
x-complete: 1
info:
  title: Google Cloud Key Management Service (KMS)
  description: manages-encryption-for-your-cloud-services-the-same-way-you-do-onpremise--you-can-generate-use-rotate-and-destroy-aes256-encryption-keys-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudkms.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:updatePrimaryVersion:
    post:
      summary: Update Version
      description: Update the version of a CryptoKey that will be used in Encrypt
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.updatePrimaryVersion
      x-api-path-slug: v1nameupdateprimaryversion-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the CryptoKey to update
      responses:
        200:
          description: OK
      tags:
      - Version