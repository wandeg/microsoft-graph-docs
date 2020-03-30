---
title: "Update shift"
description: "Update the properties of a shift object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update shift

Namespace: microsoft.graph

Update the properties of a [shift](../resources/shift.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/shifts/{shiftId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [shift](../resources/shift.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_shift"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/shifts/{shiftId}
Content-type: application/json
Content-length: 605

{
  "@odata.type": "#microsoft.graph.shift",
  "sharedShift": {
    "@odata.type": "microsoft.graph.shiftItem",
    "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
    "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "@odata.type": "#microsoft.graph.shift",
  "id": "de1527a7-27a7-de15-a727-15dea72715de",
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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
    "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
    "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
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

