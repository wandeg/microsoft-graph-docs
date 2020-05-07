---
title: "Update accessPackageResource"
description: "Update the properties of an accessPackageResource object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageResource

Namespace: microsoft.graph

Update the properties of an [accessPackageResource](../resources/accesspackageresource.md) object.

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
PATCH /accessPackageResources/{accessPackageResourcesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageResource](../resources/accesspackageresource.md) object.

The following table shows the properties that are required when you create the [accessPackageResource](../resources/accesspackageresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|url|String|**TODO: Add Description**|
|resourceType|String|**TODO: Add Description**|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|
|isPendingOnboarding|Boolean|**TODO: Add Description**|
|addedBy|String|**TODO: Add Description**|
|addedOn|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessPackageResource](../resources/accesspackageresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackageresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageResources/{accessPackageResourcesId}
Content-Type: application/json
Content-length: 319

{
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "displayName": "String",
  "description": "String",
  "url": "String",
  "resourceType": "String",
  "originId": "String",
  "originSystem": "String",
  "isPendingOnboarding": "Boolean",
  "addedBy": "String",
  "addedOn": "String (timestamp)"
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
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "id": "99437b57-7b57-9943-577b-4399577b4399",
  "displayName": "String",
  "description": "String",
  "url": "String",
  "resourceType": "String",
  "originId": "String",
  "originSystem": "String",
  "isPendingOnboarding": "Boolean",
  "addedBy": "String",
  "addedOn": "String (timestamp)"
}
```

