---
title: "Create schedule"
description: "Create a new schedule object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create schedule

Create a new [schedule](../resources/schedule.md) object.

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
POST ** Collection URI for microsoft.graph.schedule not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the schedule object.

The following table shows the properties that are required when you create the schedule.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|enabled|Boolean||
|timeZone|String||
|provisionStatus|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|provisionStatusCode|String||
|workforceIntegrationIds|String collection||
|timeClockEnabled|Boolean||
|openShiftsEnabled|Boolean||
|swapShiftsRequestsEnabled|Boolean||
|offerShiftRequestsEnabled|Boolean||
|timeOffRequestsEnabled|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [schedule](../resources/schedule.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_schedule_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.schedule not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.schedule",
  "id": "2bfb7474-7474-2bfb-7474-fb2b7474fb2b",
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

