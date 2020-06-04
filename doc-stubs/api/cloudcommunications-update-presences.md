---
title: "Update presences"
description: "Update the properties of a presences object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update presences
Namespace: microsoft.graph

Update the properties of a presences object.

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
PATCH /communications/presences
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

If successful, this method returns a `200 OK` response code and an updated [presence](../resources/presence.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_presences"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/communications/presences
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.presence",
  "id": "c26302f8-02f8-c263-f802-63c2f80263c2",
  "availability": "String",
  "activity": "String"
}
```

