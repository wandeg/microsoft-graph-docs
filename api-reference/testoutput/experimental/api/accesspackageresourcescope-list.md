---
title: "List accessPackageResourceScopes"
description: "List properties and relationships of the accessPackageResourceScope objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageResourceScopes

Namespace: microsoft.graph

List properties and relationships of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) objects.

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
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceScopes
GET /accessPackageResources/{accessPackageResourcesId}/accessPackageResourceScopes
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResourceScopes
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceScopes
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceScope](../resources/accesspackageresourcescope.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcescope"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceScopes
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageresourcescope)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 431

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageResourceScope",
      "id": "c1401591-1591-c140-9115-40c1911540c1",
      "displayName": "Display Name value",
      "description": "Description value",
      "originId": "Origin Id value",
      "originSystem": "Origin System value",
      "roleOriginId": "Role Origin Id value",
      "isRootScope": true,
      "url": "Url value"
    }
  ]
}
```

