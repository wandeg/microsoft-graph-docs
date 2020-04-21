---
title: "Update schedule"
description: "Update the properties of a schedule object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update schedule

Namespace: microsoft.graph

Update the properties of a schedule object.

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
PATCH /teams/{teamsId}/schedule
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [schedule](../resources/schedule.md) object.

The following table shows the properties that are required when you create the [schedule](../resources/schedule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|enabled|Boolean|**TODO: Add Description**|
|timeZone|String|**TODO: Add Description**|
|provisionStatus|operationStatus|**TODO: Add Description**. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|provisionStatusCode|String|**TODO: Add Description**|
|workforceIntegrationIds|String collection|**TODO: Add Description**|
|timeClockEnabled|Boolean|**TODO: Add Description**|
|openShiftsEnabled|Boolean|**TODO: Add Description**|
|swapShiftsRequestsEnabled|Boolean|**TODO: Add Description**|
|offerShiftRequestsEnabled|Boolean|**TODO: Add Description**|
|timeOffRequestsEnabled|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [schedule](../resources/schedule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_schedule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/schedule
Content-Type: application/json
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

