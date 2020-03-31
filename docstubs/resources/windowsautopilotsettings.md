---
title: "windowsAutopilotSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsAutopilotSettings resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsAutopilotSettings](../api/windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md)|Read properties and relationships of the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.|
|[Update windowsAutopilotSettings](../api/windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/windowsautopilotsettings.md)|Update the properties of a [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.|
|[sync](../api/windowsautopilotsettings-sync.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastManualSyncTriggerDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||
|syncStatus|Enumeration| Possible values are: `unknown`, `inProgress`, `completed`, `failed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```

