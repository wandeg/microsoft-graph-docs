---
title: "List accessPackageResourceRoleScopes"
description: "List properties and relationships of the accessPackageResourceRoleScope objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageResourceRoleScopes

Namespace: microsoft.graph

List properties and relationships of the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.

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
GET /accessPackageResourceRoleScopes
GET /accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes
GET /identityGovernance/entitlementManagement/accessPackageResourceRoleScopes
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageResourceRoleScopes
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescope"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageResourceRoleScopes
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
Content-Length: 371

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
      "id": "b4d40118-0118-b4d4-1801-d4b41801d4b4",
      "createdBy": "Created By value",
      "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2017-01-01T00:02:42.8886875+03:00"
    }
  ]
}
```

