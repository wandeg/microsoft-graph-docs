---
title: "List accessPackages"
description: "List properties and relationships of the accessPackage objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackages

Namespace: microsoft.graph

List properties and relationships of the [accessPackage](../resources/accesspackage.md) objects.

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
GET /accessPackages
GET /identityGovernance/entitlementManagement/accessPackages
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackages
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackages
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
Content-Length: 541

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackage",
      "id": "614bf432-f432-614b-32f4-4b6132f44b61",
      "catalogId": "Catalog Id value",
      "displayName": "Display Name value",
      "description": "Description value",
      "isHidden": true,
      "isRoleScopesVisible": true,
      "createdBy": "Created By value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00"
    }
  ]
}
```

