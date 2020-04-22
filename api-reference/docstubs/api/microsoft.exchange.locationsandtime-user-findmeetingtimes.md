---
title: "user: findMeetingTimes"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# findMeetingTimes

Namespace: microsoft.exchange.locationsAndTime

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
POST /me/findMeetingTimes
POST /users/{usersId}/findMeetingTimes
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
|attendees|[attendeeBase](../resources/microsoft.exchange.locationsandtime-attendeebase.md) collection|**TODO: Add Description**|
|locationConstraint|[locationConstraint](../resources/microsoft.exchange.locationsandtime-locationconstraint.md)|**TODO: Add Description**|
|timeConstraint|[timeConstraint](../resources/microsoft.exchange.locationsandtime-timeconstraint.md)|**TODO: Add Description**|
|meetingDuration|Duration|**TODO: Add Description**|
|maxCandidates|Int32|**TODO: Add Description**|
|isOrganizerOptional|Boolean|**TODO: Add Description**|
|returnSuggestionReasons|Boolean|**TODO: Add Description**|
|minimumAttendeePercentage|Double|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/microsoft.exchange.locationsandtime-meetingtimesuggestionsresult.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/findMeetingTimes

Content-Type: application/json
Content-length: 875

{
  "attendees": [
    {
      "@odata.type": "microsoft.exchange.locationsAndTime.attendeeBase"
    }
  ],
  "locationConstraint": {
    "@odata.type": "microsoft.exchange.locationsAndTime.locationConstraint",
    "locations": [
      {
        "@odata.type": "microsoft.exchange.locationsAndTime.locationConstraintItem",
        "resolveAvailability": true
      }
    ],
    "isRequired": true,
    "suggestLocation": true
  },
  "timeConstraint": {
    "@odata.type": "microsoft.exchange.locationsAndTime.timeConstraint",
    "activityDomain": "String",
    "timeSlots": [
      {
        "@odata.type": "microsoft.exchange.locationsAndTime.timeSlot"
      }
    ]
  },
  "meetingDuration": "PT2M36.9128186S",
  "maxCandidates": 13,
  "isOrganizerOptional": true,
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": "Double"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.exchange.locationsandtime.meetingtimesuggestionsresult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "microsoft.exchange.locationsAndTime.meetingTimeSuggestionsResult"
  }
}
```

