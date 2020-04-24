---
title: "Add responsepayload"
description: "Add responsepayload by posting to the responsepayload collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add responsepayload

Namespace: microsoft.graph

Add responsepayload by posting to the responsepayload collection.

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
POST /commands/{commandsId}/responsepayload/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [payloadResponse](../resources/payloadresponse.md) object.

The following table shows the properties that are required when you create the [payloadResponse](../resources/payloadresponse.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `204 No Content` response code and a [payloadResponse](../resources/payloadresponse.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_payloadresponse_from_payloadresponse"
}
-->
``` http
POST https://graph.microsoft.com/beta/commands/{commandsId}/responsepayload/$ref
Content-Type: application/json
Content-length: 57

{
  "@odata.type": "#microsoft.graph.payloadResponse"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.payloadresponse"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.payloadResponse",
  "id": "aab224e7-24e7-aab2-e724-b2aae724b2aa"
}
```

