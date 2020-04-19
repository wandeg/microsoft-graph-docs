---
title: "Get schedule"
description: "Read properties and relationships of a schedule object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get schedule

Namespace: microsoft.graph

Read properties and relationships of a [schedule](../resources/schedule.md) object.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule
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
If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.

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
  "@odata.type": "microsoft.graph.schedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.schedule",
    "id": "0f446dff-6dff-0f44-ff6d-440fff6d440f",
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

