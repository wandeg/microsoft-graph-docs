---
title: "Update accessPackageResourceRoleScope"
description: "Update the properties of a accessPackageResourceRoleScope object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageResourceRoleScope

Namespace: microsoft.graph

Update the properties of a [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.

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
PATCH /accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}
PATCH /accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopeId}
PATCH /identityGovernance/entitlementManagement/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopeId}
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopeId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|String||
|createdDateTime|DateTimeOffset||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackageresourcerolescope"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "createdBy": "Created By value",
  "modifiedBy": "Modified By value"
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
Content-Length: 314

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "id": "7ebcb3cd-b3cd-7ebc-cdb3-bc7ecdb3bc7e",
  "createdBy": "Created By value",
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2016-12-31T23:59:25.7728733+03:00"
}
```

