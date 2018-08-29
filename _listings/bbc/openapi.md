swagger: "2.0"
x-collection-name: BBC
x-complete: 1
info:
  title: BBC Nitro
  description: bbc-nitro-is-the-bbcs-application-programming-interface-api-for-bbc-programmes-metadata-
  termsOfService: http://www.bbc.co.uk/terms/
  contact:
    name: Open Nitro Project
    url: http://developer.bbc.co.uk/
    email: nitro@bbc.co.uk
  version: 1.0.0
host: programmes.api.bbc.com
basePath: /nitro/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /versions:
    get:
      summary: 'Metadata on editorial programme versions: original, signed, audio-described,
        etc'
      description: 'The versions feed exposes editorial "Versions" of programmes.
        These are concepts used to capture different presentations of an overall programme:
        for example, versions of a programme may include one with sign language, one
        with audio description, one edited for content and more. Versions are also
        important to understand for broadcasts: a linear broadcast or an ondemand
        is always of a specific version, not merely of a programme.'
      operationId: listVersions
      x-api-path-slug: versions-get
      parameters:
      - in: query
        name: availability
        description: filter for subset of versions that have availability
      - in: query
        name: descendants_of
        description: filter for subset of versions having given programme PID
      - in: query
        name: embargoed
        description: Control return of embargoed items (undocumented)
      - in: query
        name: media_set
        description: filter for subset of versions with availability in the given
          media set
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for versions by partner ID
      - in: query
        name: partner_pid
        description: filter for versions by partner PID
      - in: query
        name: payment_type
        description: filter for a subset of versions that are of the given payment_type
      - in: query
        name: pid
        description: filter for subset of versions having given PID
      responses:
        200:
          description: OK
      tags:
      - Versions