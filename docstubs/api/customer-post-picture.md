---
title: "Add picture"
description: "Add picture by posting to the picture collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add picture

Namespace: microsoft.graph

Add picture by posting to the picture collection.

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
POST /financials/companies/{companyId}/customers/{customerId}/picture/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [picture](../resources/picture.md) object.

The following table shows the properties that are required when you create the [picture](../resources/picture.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|width|Int32||
|height|Int32||
|contentType|String||
|content|Stream||



## Response
If successful, this method returns a `201 Created` response code and a [picture](../resources/picture.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_picture_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/customers/{customerId}/picture
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.picture",
  "width": 5,
  "height": 6,
  "contentType": "Content Type value",
  "content": "Stream"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.picture"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.picture",
  "id": "8986cb38-cb38-8986-38cb-868938cb8689",
  "width": 5,
  "height": 6,
  "contentType": "Content Type value",
  "content": "Stream"
}
```

