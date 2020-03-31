---
title: "Update calendarGroup"
description: "Update the properties of a calendarGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update calendarGroup

Namespace: microsoft.graph

Update the properties of a [calendarGroup](../resources/calendargroup.md) object.

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
PATCH /me/calendarGroups/{calendarGroupId}
PATCH /users/{usersId}/calendarGroups/{calendarGroupId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [calendarGroup](../resources/calendargroup.md) object.

The following table shows the properties that are required when you create the [calendarGroup](../resources/calendargroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|classId|Guid||
|changeKey|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [calendarGroup](../resources/calendargroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/calendarGroups/{calendarGroupId}
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "name": "Name value",
  "classId": "d0c46a8a-6a8a-d0c4-8a6a-c4d08a6ac4d0",
  "changeKey": "Change Key value"
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
Content-Length: 219

{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "id": "1513d3ee-d3ee-1513-eed3-1315eed31315",
  "name": "Name value",
  "classId": "d0c46a8a-6a8a-d0c4-8a6a-c4d08a6ac4d0",
  "changeKey": "Change Key value"
}
```

