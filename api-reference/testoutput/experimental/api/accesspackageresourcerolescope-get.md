---
title: "Get accessPackageResourceRoleScope"
description: "Read properties and relationships of the accessPackageResourceRoleScope object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessPackageResourceRoleScope

Namespace: microsoft.graph

Read properties and relationships of the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.

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
GET /accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}
GET /accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopeId}
GET /identityGovernance/entitlementManagement/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopeId}
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopeId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescope"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 345

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
    "id": "6b42e0fc-e0fc-6b42-fce0-426bfce0426b",
    "createdBy": "Created By value",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "modifiedBy": "Modified By value",
    "modifiedDateTime": "2016-12-31T23:58:13.3996216+03:00"
  }
}
```

