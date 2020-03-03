---
title: "List accessPackageResourceRoleScopes"
description: "Get the accessPackageResourceRoleScopes from the accessPackageResourceRoleScopes navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageResourceRoleScopes

Namespace: microsoft.graph

Get the accessPackageResourceRoleScopes from the accessPackageResourceRoleScopes navigation property.

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
GET /accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageResourceRoleScopes
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescope"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageresourcerolescope)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
      "id": "a5e43181-3181-a5e4-8131-e4a58131e4a5",
      "createdBy": "Created By value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00"
    }
  ]
}
```

