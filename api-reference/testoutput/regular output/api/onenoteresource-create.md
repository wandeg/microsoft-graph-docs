---
title: "Create onenoteResource"
description: "Create a new onenoteResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create onenoteResource

Namespace: microsoft.graph

Create a new [onenoteResource](../resources/onenoteresource.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/onenote/resources
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [onenoteResource](../resources/onenoteresource.md) object.

The following table shows the properties that are required when you create the [onenoteResource](../resources/onenoteresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|content|Stream||
|contentUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [onenoteResource](../resources/onenoteresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onenoteresource_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/onenote/resources
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "self": "Self value",
  "content": "Stream",
  "contentUrl": "https://example.com/contentUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "id": "be6cb2cd-b2cd-be6c-cdb2-6cbecdb26cbe",
  "self": "Self value",
  "content": "Stream",
  "contentUrl": "https://example.com/contentUrl/"
}
```

