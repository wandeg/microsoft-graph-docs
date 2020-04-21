---
title: "cloudCommunications: getPresencesByUserId"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# getPresencesByUserId

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /communications/getPresencesByUserId
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|ids|String collection|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [presence](../resources/presence.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "cloudcommunications_getpresencesbyuserid"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/getPresencesByUserId

Content-Type: application/json
Content-length: 38

{
  "ids": [
    "Ids value"
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.presence)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.presence",
      "id": "2e2f43c7-43c7-2e2f-c743-2f2ec7432f2e",
      "availability": "Availability value",
      "activity": "Activity value"
    }
  ]
}
```

