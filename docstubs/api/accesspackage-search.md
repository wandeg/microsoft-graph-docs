---
title: "Search"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Search

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /accessPackages/Search
GET /identityGovernance/entitlementManagement/accessPackages/Search
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackages/Search
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/Search
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [accessPackage](../resources/accesspackage.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "accesspackage_search"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackages/Search
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackage",
      "id": "ce7e2ce5-2ce5-ce7e-e52c-7ecee52c7ece",
      "catalogId": "Catalog Id value",
      "displayName": "Display Name value",
      "description": "Description value",
      "isHidden": true,
      "isRoleScopesVisible": true,
      "createdBy": "Created By value",
      "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2016-12-31T23:57:05.8840051+00:00"
    }
  ]
}
```

