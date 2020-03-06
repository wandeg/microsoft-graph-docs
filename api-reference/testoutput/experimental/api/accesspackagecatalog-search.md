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
GET /accessPackageCatalogs/Search
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/Search
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [accessPackageCatalog](../resources/accesspackagecatalog.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "accesspackagecatalog_search"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageCatalogs/Search
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackagecatalog)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageCatalog",
      "id": "6a9729e4-29e4-6a97-e429-976ae429976a",
      "displayName": "Display Name value",
      "description": "Description value",
      "catalogType": "Catalog Type value",
      "catalogStatus": "Catalog Status value",
      "isExternallyVisible": true,
      "createdBy": "Created By value",
      "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2016-12-31T23:58:13.3996216+03:00"
    }
  ]
}
```

