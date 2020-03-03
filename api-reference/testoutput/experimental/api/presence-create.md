---
title: "Create presence"
description: "Create a new presence object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create presence

Namespace: microsoft.graph

Create a new [presence](../resources/presence.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.presence not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [presence](../resources/presence.md) object.

The following table shows the properties that are required when you create the [presence](../resources/presence.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|availability|String||
|activity|String||



## Response
If successful, this method returns a `201 Created` response code and a [presence](../resources/presence.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_presence_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.presence not found
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.presence",
  "availability": "Availability value",
  "activity": "Activity value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.presence"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.presence",
  "id": "c99f802f-802f-c99f-2f80-9fc92f809fc9",
  "availability": "Availability value",
  "activity": "Activity value"
}
```

