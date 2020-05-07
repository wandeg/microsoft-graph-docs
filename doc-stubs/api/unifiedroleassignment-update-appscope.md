---
title: "Update appScope"
description: "Update the properties of an appScope object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update appScope

Namespace: microsoft.graph

Update the properties of an appScope object.

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
PATCH /roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}/appScope
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [appScope](../resources/appscope.md) object.

The following table shows the properties that are required when you create the [appScope](../resources/appscope.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|type|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [appScope](../resources/appscope.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_appscope"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}/appScope
Content-Type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.appScope",
  "type": "String",
  "displayName": "String"
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
  "@odata.type": "#microsoft.graph.appScope",
  "id": "a452ca0a-ca0a-a452-0aca-52a40aca52a4",
  "type": "String",
  "displayName": "String"
}
```

