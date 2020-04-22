---
title: "Create schedule"
description: "Create a new schedule object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create schedule

Namespace: microsoft.graph

Create a new schedule object.

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
POST /teams/{teamsId}/schedule
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [schedule](../resources/schedule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_schedule_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamsId}/schedule
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
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.schedule",
  "id": "e5ee1ce7-1ce7-e5ee-e71c-eee5e71ceee5",
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

