---
title: "Create itemAttachment"
description: "Create a new itemAttachment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create itemAttachment

Namespace: microsoft.graph

Create a new [itemAttachment](../resources/itemattachment.md) object.

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
POST ** Collection URI for microsoft.graph.itemAttachment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [itemAttachment](../resources/itemattachment.md) object.

The following table shows the properties that are required when you create the [itemAttachment](../resources/itemattachment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [attachment](../resources/attachment.md)|
|name|String| Inherited from [attachment](../resources/attachment.md)|
|contentType|String| Inherited from [attachment](../resources/attachment.md)|
|size|Int32| Inherited from [attachment](../resources/attachment.md)|
|isInline|Boolean| Inherited from [attachment](../resources/attachment.md)|



## Response
If successful, this method returns a `201 Created` response code and a [itemAttachment](../resources/itemattachment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_itemattachment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.itemAttachment not found
Content-type: application/json
Content-length: 156

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemattachment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 267

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "id": "06f99630-9630-06f9-3096-f9063096f906",
  "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true
}
```

