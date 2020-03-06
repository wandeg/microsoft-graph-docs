---
title: "Update shiftPreferences"
description: "Update the properties of a shiftPreferences object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update shiftPreferences

Namespace: microsoft.graph

Update the properties of a [shiftPreferences](../resources/shiftpreferences.md) object.

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
PATCH /me/settings/shiftPreferences
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [shiftPreferences](../resources/shiftpreferences.md) object.

The following table shows the properties that are required when you create the [shiftPreferences](../resources/shiftpreferences.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|availability|[shiftAvailability](../resources/shiftavailability.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [shiftPreferences](../resources/shiftpreferences.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_shiftpreferences"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/settings/shiftPreferences
Content-type: application/json
Content-length: 1102

{
  "@odata.type": "#microsoft.graph.shiftPreferences",
  "availability": [
    {
      "@odata.type": "microsoft.graph.shiftAvailability",
      "recurrence": {
        "@odata.type": "microsoft.graph.patternedRecurrence",
        "pattern": {
          "@odata.type": "microsoft.graph.recurrencePattern",
          "type": "String",
          "interval": 8,
          "month": 5,
          "dayOfMonth": 10,
          "daysOfWeek": [
            "String"
          ],
          "firstDayOfWeek": "String",
          "index": "String"
        },
        "range": {
          "@odata.type": "microsoft.graph.recurrenceRange",
          "type": "String",
          "startDate": "Date",
          "endDate": "Date",
          "recurrenceTimeZone": "Recurrence Time Zone value",
          "numberOfOccurrences": 3
        }
      },
      "timeZone": "Time Zone value",
      "timeSlots": [
        {
          "@odata.type": "microsoft.graph.timeRange",
          "startTime": "12:00:03.0490000",
          "endTime": "11:57:54.2000000"
        }
      ]
    }
  ]
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
Content-Length: 1647

{
  "@odata.type": "#microsoft.graph.shiftPreferences",
  "id": "b7355a65-5a65-b735-655a-35b7655a35b7",
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
  "availability": [
    {
      "@odata.type": "microsoft.graph.shiftAvailability",
      "recurrence": {
        "@odata.type": "microsoft.graph.patternedRecurrence",
        "pattern": {
          "@odata.type": "microsoft.graph.recurrencePattern",
          "type": "String",
          "interval": 8,
          "month": 5,
          "dayOfMonth": 10,
          "daysOfWeek": [
            "String"
          ],
          "firstDayOfWeek": "String",
          "index": "String"
        },
        "range": {
          "@odata.type": "microsoft.graph.recurrenceRange",
          "type": "String",
          "startDate": "Date",
          "endDate": "Date",
          "recurrenceTimeZone": "Recurrence Time Zone value",
          "numberOfOccurrences": 3
        }
      },
      "timeZone": "Time Zone value",
      "timeSlots": [
        {
          "@odata.type": "microsoft.graph.timeRange",
          "startTime": "12:00:03.0490000",
          "endTime": "11:57:54.2000000"
        }
      ]
    }
  ]
}
```

