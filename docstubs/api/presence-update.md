---
title: "Update presence"
description: "Update the properties of a presence object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update presence

Namespace: microsoft.graph

Update the properties of a [presence](../resources/presence.md) object.

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
PATCH /me/presence
PATCH /users/{usersId}/presence
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [presence](../resources/presence.md) object.

The following table shows the properties that are required when you create the [presence](../resources/presence.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|availability|String||
|activity|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [presence](../resources/presence.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_presence"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/presence
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.presence",
  "id": "065df731-f731-065d-31f7-5d0631f75d06",
  "availability": "Availability value",
  "activity": "Activity value"
}
```

