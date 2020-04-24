---
title: "Create accessPackageAssignmentResourceRole"
description: "Create a new accessPackageAssignmentResourceRole object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageAssignmentResourceRole

Namespace: microsoft.graph

Create a new [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.

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
POST /accessPackageAssignmentResourceRoles
POST /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentresourcerole_from_accesspackageassignmentresourceroles"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageAssignmentResourceRoles
Content-Type: application/json
Content-length: 182

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "status": "Status value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageassignmentresourcerole"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "id": "88e0ab46-ab46-88e0-46ab-e08846abe088",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "status": "Status value"
}
```

