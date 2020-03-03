---
title: "win32LobAppRestartSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# win32LobAppRestartSettings resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|countdownDisplayBeforeRestartInMinutes|Int32|The number of minutes before the restart time to display the countdown dialog for pending restarts.|
|gracePeriodInMinutes|Int32|The number of minutes to wait before restarting the device after an app installation.|
|restartNotificationSnoozeDurationInMinutes|Int32|The number of minutes to snooze the restart notification dialog when the snooze button is selected.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRestartSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRestartSettings",
  "gracePeriodInMinutes": 1024,
  "countdownDisplayBeforeRestartInMinutes": 1024,
  "restartNotificationSnoozeDurationInMinutes": 1024
}
```

