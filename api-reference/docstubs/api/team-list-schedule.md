---
title: "List schedule"
description: "Get the schedules from the schedule navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List schedule

Namespace: microsoft.graph

Get the schedules from the schedule navigation property.

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
GET /teams/{teamsId}/schedule
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
If successful, this method returns a `200 OK` response code and a collection of [schedule](../resources/schedule.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_schedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/schedule
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.schedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.schedule",
      "id": "04b6e246-e246-04b6-46e2-b60446e2b604",
      "enabled": true,
      "timeZone": "Time Zone value",
      "provisionStatus": "String",
      "provisionStatusCode": "Provision Status Code value",
      "workforceIntegrationIds": [
        "Workforce Integration Ids value"
      ],
      "timeClockEnabled": true,
      "openShiftsEnabled": true,
      "swapShiftsRequestsEnabled": true,
      "offerShiftRequestsEnabled": true,
      "timeOffRequestsEnabled": true
    }
  ]
}
```

