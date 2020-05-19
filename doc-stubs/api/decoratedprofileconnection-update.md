---
title: "Update DecoratedProfileConnection"
description: "Update the properties of a DecoratedProfileConnection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update DecoratedProfileConnection

Namespace: microsoft.graph

Update the properties of a [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.

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
PATCH /decoratedProfileConnections/{decoratedProfileConnectionsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.

The following table shows the properties that are required when you create the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|relevanceScore|Double|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_decoratedprofileconnection"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/decoratedProfileConnections/{decoratedProfileConnectionsId}
Content-Type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.DecoratedProfileConnection",
  "relevanceScore": "Double"
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
  "@odata.type": "#microsoft.graph.DecoratedProfileConnection",
  "id": "a9e5f845-f845-a9e5-45f8-e5a945f8e5a9",
  "relevanceScore": "Double"
}
```

