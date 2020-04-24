---
title: "Create accessPackageResourceRoleScopes"
description: "Create a new accessPackageResourceRoleScopes object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageResourceRoleScopes

Namespace: microsoft.graph

Create a new accessPackageResourceRoleScopes object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackageresourcerolescopes"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackages/{accessPackagesId}/accessPackageResourceRoleScopes
Content-Type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "createdBy": "Created By value",
  "modifiedBy": "Modified By value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresourcerolescope"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "id": "9e45ef00-ef00-9e45-00ef-459e00ef459e",
  "createdBy": "Created By value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00"
}
```

