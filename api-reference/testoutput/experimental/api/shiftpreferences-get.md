---
title: "Get shiftPreferences"
description: "Read properties and relationships of the shiftPreferences object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get shiftPreferences

Namespace: microsoft.graph

Read properties and relationships of the [shiftPreferences](../resources/shiftpreferences.md) object.

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
GET /me/settings/shiftPreferences
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [shiftPreferences](../resources/shiftpreferences.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_shiftpreferences"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/settings/shiftPreferences
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shiftPreferences"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1773

{
  "value": {
    "@odata.type": "#microsoft.graph.shiftPreferences",
    "id": "4aa2d663-d663-4aa2-63d6-a24a63d6a24a",
    "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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
            "startTime": "12:02:50.6370000",
            "endTime": "12:02:54.9570000"
          }
        ]
      }
    ]
  }
}
```

