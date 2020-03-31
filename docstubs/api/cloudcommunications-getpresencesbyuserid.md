---
title: "getPresencesByUserId"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getPresencesByUserId

Namespace: microsoft.graph



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
POST /communications/getPresencesByUserId
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|ids|String collection||



## Response
If successful, this action returns a `200 OK` response code and a [presence](../resources/presence.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "cloudcommunications_getpresencesbyuserid"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/getPresencesByUserId

Content-type: application/json
Content-length: 38

{
  "ids": [
    "Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.presence)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.presence",
      "id": "f60edeab-deab-f60e-abde-0ef6abde0ef6",
      "availability": "Availability value",
      "activity": "Activity value"
    }
  ]
}
```

