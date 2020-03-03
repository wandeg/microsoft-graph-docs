---
title: "List accessPackageResourceRoles"
description: "List properties and relationships of the accessPackageResourceRole objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageResourceRoles

Namespace: microsoft.graph

List properties and relationships of the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects.

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
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceRoles
GET /accessPackageResources/{accessPackageResourcesId}/accessPackageResourceRoles
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResourceRoles
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceRoles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerole"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceRoles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageresourcerole)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageResourceRole",
      "id": "d54e2aed-2aed-d54e-ed2a-4ed5ed2a4ed5",
      "displayName": "Display Name value",
      "description": "Description value",
      "originId": "Origin Id value",
      "originSystem": "Origin System value"
    }
  ]
}
```

