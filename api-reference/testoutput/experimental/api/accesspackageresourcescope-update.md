---
title: "Update accessPackageResourceScope"
description: "Update the properties of a accessPackageResourceScope object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageResourceScope

Namespace: microsoft.graph

Update the properties of a [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.

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
PATCH /accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}/accessPackageResourceScope
PATCH /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageResourceScope
PATCH /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceScopes/{accessPackageResourceScopeId}
PATCH /accessPackageResources/{accessPackageResourcesId}/accessPackageResourceScopes/{accessPackageResourceScopeId}
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResourceScopes/{accessPackageResourceScopeId}
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceScopes/{accessPackageResourceScopeId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}/accessPackageResourceScope
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopeId}/accessPackageResourceScope
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceScope](../resources/accesspackageresourcescope.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|originId|String||
|originSystem|String||
|roleOriginId|String||
|isRootScope|Boolean||
|url|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackageresourcescope"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}/accessPackageResourceScope
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "displayName": "Display Name value",
  "description": "Description value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "roleOriginId": "Role Origin Id value",
  "isRootScope": true,
  "url": "Url value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 362

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
```

