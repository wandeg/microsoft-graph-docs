---
title: "Create DecoratedProfileConnection"
description: "Create a new DecoratedProfileConnection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create DecoratedProfileConnection

Namespace: microsoft.graph

Create a new [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.

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
POST /decoratedProfileConnections
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.

The following table shows the properties that are required when you create the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|relevanceScore|Double||



## Response
If successful, this method returns a `201 Created` response code and a [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_decoratedprofileconnection_from_decoratedprofileconnections"
}
-->
``` http
POST https://graph.microsoft.com/beta/decoratedProfileConnections
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.DecoratedProfileConnection",
  "relevanceScore": "Double"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.decoratedprofileconnection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 148

{
  "@odata.type": "#microsoft.graph.DecoratedProfileConnection",
  "id": "4fdfd2e2-d2e2-4fdf-e2d2-df4fe2d2df4f",
  "relevanceScore": "Double"
}
```

