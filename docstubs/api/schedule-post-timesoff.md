---
title: "Add timesOff"
description: "Add timesOff by posting to the timesOff collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add timesOff

Namespace: microsoft.graph

Add timesOff by posting to the timesOff collection.

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
POST /me/joinedGroups/{groupId}/team/schedule/timesOff/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_timeoff_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timesOff
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.timeOff",
  "sharedTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem",
    "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
    "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.timeoff"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 971

{
  "@odata.type": "#microsoft.graph.timeOff",
  "id": "0e9a1fd2-1fd2-0e9a-d21f-9a0ed21f9a0e",
  "createdDateTime": "2016-12-31T23:56:52.9286964+00:00",
  "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00",
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
    "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
    "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
    "theme": "String",
    "timeOffReasonId": "Time Off Reason Id value"
  },
  "draftTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "userId": "User Id value"
}
```

