---
title: "Get shiftPreferences"
description: "Read the properties and relationships of a shiftPreferences object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get shiftPreferences

Namespace: microsoft.graph

Read the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.

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
GET /invitations/{invitationsId}/invitedUser/settings/shiftPreferences
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_shiftpreferences"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/settings/shiftPreferences
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shiftPreferences"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.shiftPreferences",
    "id": "f64dd876-d876-f64d-76d8-4df676d84df6",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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
            "startTime": "11:58:07.5130000",
            "endTime": "11:57:24.1090000"
          }
        ]
      }
    ]
  }
}
```

