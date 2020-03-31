---
title: "Add shifts"
description: "Add shifts by posting to the shifts collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add shifts

Namespace: microsoft.graph

Add shifts by posting to the shifts collection.

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
POST /me/joinedGroups/{groupId}/team/schedule/shifts/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [shift](../resources/shift.md) object.

The following table shows the properties that are required when you create the [shift](../resources/shift.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|sharedShift|[shiftItem](../resources/shiftitem.md)||
|draftShift|[shiftItem](../resources/shiftitem.md)||
|userId|String||
|schedulingGroupId|String||



## Response
If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_shift_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/shifts
Content-type: application/json
Content-length: 605

{
  "@odata.type": "#microsoft.graph.shift",
  "sharedShift": {
    "@odata.type": "microsoft.graph.shiftItem",
    "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
    "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
    "theme": "String",
    "notes": "Notes value",
    "activities": [
      {
        "@odata.type": "microsoft.graph.shiftActivity",
        "isPaid": true,
        "code": "Code value"
      }
    ]
  },
  "draftShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "userId": "User Id value",
  "schedulingGroupId": "Scheduling Group Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1150

{
  "@odata.type": "#microsoft.graph.shift",
  "id": "097928d8-28d8-0979-d828-7909d8287909",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "sharedShift": {
    "@odata.type": "microsoft.graph.shiftItem",
    "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
    "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
    "theme": "String",
    "notes": "Notes value",
    "activities": [
      {
        "@odata.type": "microsoft.graph.shiftActivity",
        "isPaid": true,
        "code": "Code value"
      }
    ]
  },
  "draftShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "userId": "User Id value",
  "schedulingGroupId": "Scheduling Group Id value"
}
```

