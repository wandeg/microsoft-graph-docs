---
title: "Create presence"
description: "Create a new presence object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create presence

Namespace: microsoft.graph

Create a new presence object.

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
POST /me/presence
POST /users/{usersId}/presence
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [presence](../resources/presence.md) object.

The following table shows the properties that are required when you create the [presence](../resources/presence.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|availability|String|**TODO: Add Description**|
|activity|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [presence](../resources/presence.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_presence_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/presence
Content-Type: application/json
Content-length: 104

{
  "@odata.type": "#microsoft.graph.presence",
  "availability": "String",
  "activity": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.presence"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.presence",
  "id": "563a26ec-26ec-563a-ec26-3a56ec263a56",
  "availability": "String",
  "activity": "String"
}
```

