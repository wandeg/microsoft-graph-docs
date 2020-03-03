---
title: "List accessPackageCatalogs"
description: "Get the accessPackageCatalogs from the accessPackageCatalogs navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageCatalogs

Namespace: microsoft.graph

Get the accessPackageCatalogs from the accessPackageCatalogs navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}
-->
``` http
GET https://graph.microsoft.com/localtest/identityGovernance/entitlementManagement/accessPackageCatalogs
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
Content-Length: 575

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageCatalog",
      "id": "200673a9-73a9-2006-a973-0620a9730620",
      "displayName": "Display Name value",
      "description": "Description value",
      "catalogType": "Catalog Type value",
      "catalogStatus": "Catalog Status value",
      "isExternallyVisible": true,
      "createdBy": "Created By value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00"
    }
  ]
}
```

