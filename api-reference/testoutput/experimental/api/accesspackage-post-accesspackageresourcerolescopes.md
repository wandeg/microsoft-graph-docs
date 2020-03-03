---
title: "Add accessPackageResourceRoleScopes"
description: "Add accessPackageResourceRoleScopes by posting to the accessPackageResourceRoleScopes collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageResourceRoleScopes

Namespace: microsoft.graph

Add accessPackageResourceRoleScopes by posting to the accessPackageResourceRoleScopes collection.

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
POST /accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes/$ref
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageResourceRoleScopes/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
POST https://graph.microsoft.com/localtest/accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes
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
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "id": "a5e43181-3181-a5e4-8131-e4a58131e4a5",
  "createdBy": "Created By value",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00"
}
```

