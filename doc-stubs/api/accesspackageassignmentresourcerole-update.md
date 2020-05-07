---
title: "Update accessPackageAssignmentResourceRole"
description: "Update the properties of an accessPackageAssignmentResourceRole object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageAssignmentResourceRole

Namespace: microsoft.graph

Update the properties of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.

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
PATCH /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentresourcerole"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}
Content-Type: application/json
Content-length: 154

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "id": "711cda86-da86-711c-86da-1c7186da1c71",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

