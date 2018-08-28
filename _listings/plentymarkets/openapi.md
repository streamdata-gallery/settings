swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/markets/settings:
    get:
      summary: List market settings
      description: Lists market settings. The marketplace ID and the type must be
        specified.
      operationId: getRestMarketsSettings
      x-api-path-slug: restmarketssettings-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Market
      - Settings
    post:
      summary: Create market settings
      description: Creates new market settings by given data. The marketplace ID and
        the type must be specified.
      operationId: postRestMarketsSettings
      x-api-path-slug: restmarketssettings-post
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
  /rest/markets/settings/bulk:
    post:
      summary: Create market settings
      description: Creates new market settings by given data. The marketplace ID and
        the type must be specified.
      operationId: postRestMarketsSettingsBulk
      x-api-path-slug: restmarketssettingsbulk-post
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    put:
      summary: Update market settings
      description: Updates market settings. The market settings ID must be specified.
      operationId: putRestMarketsSettingsBulk
      x-api-path-slug: restmarketssettingsbulk-put
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
  /rest/markets/settings/{settingId}:
    delete:
      summary: Delete market settings
      description: Deletes market settings. The market settings ID must be specified.
      operationId: deleteRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-delete
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    get:
      summary: Get market settings
      description: Gets market settings. The market settings ID must be specified.
      operationId: getRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-get
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    put:
      summary: Update market settings
      description: Updates market settings. The market settings ID must be specified.
      operationId: putRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-put
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings