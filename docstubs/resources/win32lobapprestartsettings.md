---
title: "win32LobAppRestartSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# win32LobAppRestartSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|countdownDisplayBeforeRestartInMinutes|Int32||
|gracePeriodInMinutes|Int32||
|restartNotificationSnoozeDurationInMinutes|Int32||

## Relationships
None

## JSON representation
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

