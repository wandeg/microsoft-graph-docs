---
title: "Create accessPackageResourceRoleScope"
description: "Create a new accessPackageResourceRoleScope object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create accessPackageResourceRoleScope

Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.

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
POST /accessPackageResourceRoleScopes
POST /accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes
POST /identityGovernance/entitlementManagement/accessPackageResourceRoleScopes
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageResourceRoleScopes
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the accessPackageResourceRoleScope object.

The following table shows the properties that are required when you create the accessPackageResourceRoleScope.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|String||
|createdDateTime|DateTimeOffset||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackageresourcerolescopes"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/accessPackageResourceRoleScopes
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
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresourcerolescope"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 314

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "id": "c768d37d-d37d-c768-7dd3-68c77dd368c7",
  "createdBy": "Created By value",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:03:12.7204145+03:00"
}
```

