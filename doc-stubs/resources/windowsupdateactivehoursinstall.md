---
title: "windowsUpdateActiveHoursInstall resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsUpdateActiveHoursInstall resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [windowsUpdateInstallScheduleType](../resources/windowsupdateinstallscheduletype.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeHoursEnd|TimeOfDay|**TODO: Add Description**|
|activeHoursStart|TimeOfDay|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```

