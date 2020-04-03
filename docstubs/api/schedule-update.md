---
title: "Update schedule"
description: "Update the properties of a schedule object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update schedule

Namespace: microsoft.graph

Update the properties of a [schedule](../resources/schedule.md) object.

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
PATCH /teams/{teamsId}/schedule
PATCH /me/joinedGroups/{groupId}/team/schedule
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [schedule](../resources/schedule.md) object.

The following table shows the properties that are required when you create the [schedule](../resources/schedule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|enabled|Boolean||
|timeZone|String||
|provisionStatus|Enumeration| Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|provisionStatusCode|String||
|workforceIntegrationIds|String collection||
|timeClockEnabled|Boolean||
|openShiftsEnabled|Boolean||
|swapShiftsRequestsEnabled|Boolean||
|offerShiftRequestsEnabled|Boolean||
|timeOffRequestsEnabled|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [schedule](../resources/schedule.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_schedule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/schedule
Content-type: application/json
Content-length: 440

{
  "@odata.type": "#microsoft.graph.schedule",
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
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.schedule",
  "id": "29b94298-4298-29b9-9842-b9299842b929",
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
```

