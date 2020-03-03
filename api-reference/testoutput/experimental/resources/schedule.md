---
title: "schedule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# schedule resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List schedules](../api/schedule-list.md)|[schedule](../resources/schedule.md) collection|List properties and relationships of the [schedule](../resources/schedule.md) objects.|
|[Get schedule](../api/schedule-get.md)|[schedule](../resources/schedule.md)|Read properties and relationships of the [schedule](../resources/schedule.md) object.|
|[Create schedule](../api/schedule-create.md)|[schedule](../resources/schedule.md)|Create a new [schedule](../resources/schedule.md) object.|
|[Delete schedule](../api/schedule-delete.md)|None|Deletes a [schedule](../resources/schedule.md).|
|[Update schedule](../api/schedule-update.md)|[schedule](../resources/schedule.md)|Update the properties of a [schedule](../resources/schedule.md) object.|
|[share](../api/schedule-share.md)|None||
|[List shifts](../api/schedule-list-shifts.md)|[shift](../resources/shift.md) collection|Get the shifts from the shifts navigation property.|
|[Add shifts](../api/schedule-post-shifts.md)|[shift](../resources/shift.md)|Add shifts by posting to the shifts collection.|
|[List openShifts](../api/schedule-list-openshifts.md)|[openShift](../resources/openshift.md) collection|Get the openShifts from the openShifts navigation property.|
|[Add openShifts](../api/schedule-post-openshifts.md)|[openShift](../resources/openshift.md)|Add openShifts by posting to the openShifts collection.|
|[List timesOff](../api/schedule-list-timesoff.md)|[timeOff](../resources/timeoff.md) collection|Get the timeOffs from the timesOff navigation property.|
|[Add timesOff](../api/schedule-post-timesoff.md)|[timeOff](../resources/timeoff.md)|Add timesOff by posting to the timesOff collection.|
|[List timeOffReasons](../api/schedule-list-timeoffreasons.md)|[timeOffReason](../resources/timeoffreason.md) collection|Get the timeOffReasons from the timeOffReasons navigation property.|
|[Add timeOffReasons](../api/schedule-post-timeoffreasons.md)|[timeOffReason](../resources/timeoffreason.md)|Add timeOffReasons by posting to the timeOffReasons collection.|
|[List schedulingGroups](../api/schedule-list-schedulinggroups.md)|[schedulingGroup](../resources/schedulinggroup.md) collection|Get the schedulingGroups from the schedulingGroups navigation property.|
|[Add schedulingGroups](../api/schedule-post-schedulinggroups.md)|[schedulingGroup](../resources/schedulinggroup.md)|Add schedulingGroups by posting to the schedulingGroups collection.|
|[List swapShiftsChangeRequests](../api/schedule-list-swapshiftschangerequests.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) collection|Get the swapShiftsChangeRequests from the swapShiftsChangeRequests navigation property.|
|[Add swapShiftsChangeRequests](../api/schedule-post-swapshiftschangerequests.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)|Add swapShiftsChangeRequests by posting to the swapShiftsChangeRequests collection.|
|[List openShiftChangeRequests](../api/schedule-list-openshiftchangerequests.md)|[openShiftChangeRequest](../resources/openshiftchangerequest.md) collection|Get the openShiftChangeRequests from the openShiftChangeRequests navigation property.|
|[Add openShiftChangeRequests](../api/schedule-post-openshiftchangerequests.md)|[openShiftChangeRequest](../resources/openshiftchangerequest.md)|Add openShiftChangeRequests by posting to the openShiftChangeRequests collection.|
|[List offerShiftRequests](../api/schedule-list-offershiftrequests.md)|[offerShiftRequest](../resources/offershiftrequest.md) collection|Get the offerShiftRequests from the offerShiftRequests navigation property.|
|[Add offerShiftRequests](../api/schedule-post-offershiftrequests.md)|[offerShiftRequest](../resources/offershiftrequest.md)|Add offerShiftRequests by posting to the offerShiftRequests collection.|
|[List timeOffRequests](../api/schedule-list-timeoffrequests.md)|[timeOffRequest](../resources/timeoffrequest.md) collection|Get the timeOffRequests from the timeOffRequests navigation property.|
|[Add timeOffRequests](../api/schedule-post-timeoffrequests.md)|[timeOffRequest](../resources/timeoffrequest.md)|Add timeOffRequests by posting to the timeOffRequests collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|enabled|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|offerShiftRequestsEnabled|Boolean||
|openShiftsEnabled|Boolean||
|provisionStatus|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|provisionStatusCode|String||
|swapShiftsRequestsEnabled|Boolean||
|timeClockEnabled|Boolean||
|timeOffRequestsEnabled|Boolean||
|timeZone|String||
|workforceIntegrationIds|String collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|offerShiftRequests|[offerShiftRequest](../resources/offershiftrequest.md) collection||
|openShiftChangeRequests|[openShiftChangeRequest](../resources/openshiftchangerequest.md) collection||
|openShifts|[openShift](../resources/openshift.md) collection||
|schedulingGroups|[schedulingGroup](../resources/schedulinggroup.md) collection||
|shifts|[shift](../resources/shift.md) collection||
|swapShiftsChangeRequests|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) collection||
|timeOffReasons|[timeOffReason](../resources/timeoffreason.md) collection||
|timeOffRequests|[timeOffRequest](../resources/timeoffrequest.md) collection||
|timesOff|[timeOff](../resources/timeoff.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.schedule",
  "id": "String (identifier)",
  "enabled": true,
  "timeZone": "String",
  "provisionStatus": "String",
  "provisionStatusCode": "String",
  "workforceIntegrationIds": [
    "String"
  ],
  "timeClockEnabled": true,
  "openShiftsEnabled": true,
  "swapShiftsRequestsEnabled": true,
  "offerShiftRequestsEnabled": true,
  "timeOffRequestsEnabled": true
}
```

