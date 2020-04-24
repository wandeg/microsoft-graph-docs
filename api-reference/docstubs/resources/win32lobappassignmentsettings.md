---
title: "win32LobAppAssignmentSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppAssignmentSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [mobileAppAssignmentSettings](../resources/mobileappassignmentsettings.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deliveryOptimizationPriority|win32LobAppDeliveryOptimizationPriority|The delivery optimization priority for this app assignment. This setting is not supported in National Cloud environments. Possible values are: `notConfigured`, `foreground`.|
|installTimeSettings|[mobileAppInstallTimeSettings](../resources/mobileappinstalltimesettings.md)|The install time settings to apply for this app assignment.|
|notifications|win32LobAppNotification|The notification status for this app assignment. Possible values are: `showAll`, `showReboot`, `hideAll`.|
|restartSettings|[win32LobAppRestartSettings](../resources/win32lobapprestartsettings.md)|The reboot settings to apply for this app assignment.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String",
  "restartSettings": {
    "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
    "gracePeriodInMinutes": 1024,
    "countdownDisplayBeforeRestartInMinutes": 1024,
    "restartNotificationSnoozeDurationInMinutes": 1024
  },
  "installTimeSettings": {
    "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
    "useLocalTime": true,
    "startDateTime": "String (timestamp)",
    "deadlineDateTime": "String (timestamp)"
  },
  "deliveryOptimizationPriority": "String"
}
```

