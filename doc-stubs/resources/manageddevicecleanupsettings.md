---
title: "managedDeviceCleanupSettings resource type"
description: "Define the rule when the admin wants the devices to be cleaned up."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceCleanupSettings resource type


Namespace: microsoft.graph

Define the rule when the admin wants the devices to be cleaned up.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceInactivityBeforeRetirementInDays|String|Number of days when the device has not contacted Intune.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```

