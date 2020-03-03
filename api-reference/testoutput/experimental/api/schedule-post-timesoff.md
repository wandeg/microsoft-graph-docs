---
title: "Add timesOff"
description: "Add timesOff by posting to the timesOff collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add timesOff

Add timesOff by posting to the timesOff collection.

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
POST /me/joinedGroups/{groupId}/team/schedule/timesOff/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the timeOff object.

The following table shows the properties that are required when you create the timeOff.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|sharedTimeOff|[timeOffItem](../resources/timeOffItem.md)||
|draftTimeOff|[timeOffItem](../resources/timeOffItem.md)||
|userId|String||



## Response
If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_timeoff_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/team/schedule/timesOff
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.timeOff",
  "sharedTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem",
    "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
    "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
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
  "id": "59027fba-7fba-5902-ba7f-0259ba7f0259",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
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
    "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
    "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
    "theme": "String",
    "timeOffReasonId": "Time Off Reason Id value"
  },
  "draftTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "userId": "User Id value"
}
```

