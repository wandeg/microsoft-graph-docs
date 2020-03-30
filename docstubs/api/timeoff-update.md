---
title: "Update timeOff"
description: "Update the properties of a timeOff object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update timeOff

Namespace: microsoft.graph

Update the properties of a [timeOff](../resources/timeoff.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/timesOff/{timeOffId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [timeOff](../resources/timeoff.md) object.

The following table shows the properties that are required when you create the [timeOff](../resources/timeoff.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|sharedTimeOff|[timeOffItem](../resources/timeoffitem.md)||
|draftTimeOff|[timeOffItem](../resources/timeoffitem.md)||
|userId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [timeOff](../resources/timeoff.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_timeoff"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timesOff/{timeOffId}
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.timeOff",
  "sharedTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem",
    "startDateTime": "2016-12-31T23:57:02.6825424+00:00",
    "endDateTime": "2016-12-31T23:59:12.2321935+00:00",
    "theme": "String",
    "timeOffReasonId": "Time Off Reason Id value"
  },
  "draftTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "userId": "User Id value"
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
Content-Length: 971

{
  "@odata.type": "#microsoft.graph.timeOff",
  "id": "a6d3ca0c-ca0c-a6d3-0cca-d3a60ccad3a6",
  "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
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
  "sharedTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem",
    "startDateTime": "2016-12-31T23:57:02.6825424+00:00",
    "endDateTime": "2016-12-31T23:59:12.2321935+00:00",
    "theme": "String",
    "timeOffReasonId": "Time Off Reason Id value"
  },
  "draftTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "userId": "User Id value"
}
```

