---
title: "Update shiftPreferences"
description: "Update the properties of a shiftPreferences object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update shiftPreferences

Namespace: microsoft.graph

Update the properties of a [shiftPreferences](../resources/shiftpreferences.md) object.

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
PATCH /invitations/{invitationsId}/invitedUser/settings/shiftPreferences
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [shiftPreferences](../resources/shiftpreferences.md) object.

The following table shows the properties that are required when you create the [shiftPreferences](../resources/shiftpreferences.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|availability|[shiftAvailability](../resources/shiftavailability.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [shiftPreferences](../resources/shiftpreferences.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_shiftpreferences"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/settings/shiftPreferences
Content-Type: application/json
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
          "startTime": "11:58:07.5130000",
          "endTime": "11:57:24.1090000"
        }
      ]
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

