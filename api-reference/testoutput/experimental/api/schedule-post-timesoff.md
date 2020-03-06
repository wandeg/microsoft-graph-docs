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
|Header|Value|
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
POST https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/team/schedule/timesOff
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.timeOff",
  "sharedTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem",
    "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
    "endDateTime": "2017-01-01T00:02:18.392989+03:00",
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
Content-Length: 970

{
  "@odata.type": "#microsoft.graph.timeOff",
  "id": "422a3bc0-3bc0-422a-c03b-2a42c03b2a42",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
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
    "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
    "endDateTime": "2017-01-01T00:02:18.392989+03:00",
    "theme": "String",
    "timeOffReasonId": "Time Off Reason Id value"
  },
  "draftTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "userId": "User Id value"
}
```

