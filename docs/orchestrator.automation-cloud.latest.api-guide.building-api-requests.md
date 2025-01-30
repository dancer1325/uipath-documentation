https://docs.uipath.com/orchestrator/automation-cloud/latest/api-guide/building-api-requests

* Orchestrator API calls
  * -- via -- HTTP methods | Orchestrator base URL
    * https://cloud.uipath.com/{organizationName}/{tenantName}/orchestrator_
      * Orchestrator base URL
  * ⚠️if you want to access resources | folder -> ADD request headers `FolderId` + `FolderPath` + `FolderKey` ⚠️/
    * `FolderId`
      * ways to obtain it
        * GET  /odata/Folders
        * Orchestrator URL
          * _Example:_ https://your-domain-server.com/?fid=2032&tid=8
      * type Int 64
      * ⚠️if you change the licensing plan | your Orchestrator account -> `FolderId` value changes ⚠️
    * `FolderKey`
      * ways to obtain it
        * GET /odata/Folders
        * type Unique Id/String
      * ⚠️if you change the licensing plan | your Orchestrator account -> FolderKey value remains the same ⚠️
    * ways to send
      * encoded ( -- via -- Base64 UTF-16LE encoding) or
        * _Example:_ `X-UIPATH-FolderPath-Encoded "{Encoded FolderPath value}"`
      * plain text
        * _Examples:_
          * `X-UIPATH-OrganizationUnitId "FolderId"`
          * `X-UIPATH-FolderPath "PlainText FolderPath value"`
          * `X-UIPATH-FolderKey "FolderKey"`
    * if you use relative folder paths -> use request header `X-UIPATH-FolderPath-Encoded` header /
      * if path starts with "/" -> starts | root folder of the tree the ambient folder is part of
      * if path starts with "." == starts | ambient folder
      * if path starts with ".." == starts | one level up in the hierarchy of the ambient folder
      * ❌trailing slashes ("..../") NOT accepted ❌

* GET requests
  * 👀generic ALLOWED [OData](orchestrator.automation-cloud.latest.api-guide.about-odata-and-references.md) clauses 👀
    * `$top`
      * limit the amount of data / you retrieve
      * _Example:_ https://cloud.uipath.com/{organizationName}/{tenantName}/orchestrator_/odata/Environments?$top=10 returns the first 10 environments available | Community Edition of Orchestrator
    * `$filter`
      * TODO:
    * `$expand`
    * `$select`
    * `$orderby`
    * `$skip`

* POST requests

* PUT requests

* PATCH requests

* DELETE requests