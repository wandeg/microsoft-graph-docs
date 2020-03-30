---
title: "Get schedule"
description: "Read properties and relationships of the schedule object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get schedule

Namespace: microsoft.graph

Read properties and relationships of the [schedule](../resources/schedule.md) object.

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
GET /teams/{teamsId}/schedule
GET /me/joinedGroups/{groupId}/team/schedule
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [schedule](../resources/schedule.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_schedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/schedule
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": {
    "@odata.type": "#microsoft.graph.schedule",
    "id": "3f8e0e85-0e85-3f8e-850e-8e3f850e8e3f",
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
}
```

