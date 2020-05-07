---
title: "deviceManagementIntentDeviceSettingStateSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementIntentDeviceSettingStateSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantCount|Int32|**TODO: Add Description**|
|conflictCount|Int32|**TODO: Add Description**|
|errorCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|nonCompliantCount|Int32|**TODO: Add Description**|
|notApplicableCount|Int32|**TODO: Add Description**|
|remediatedCount|Int32|**TODO: Add Description**|
|settingName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "compliantCount": "Integer",
  "conflictCount": "Integer",
  "errorCount": "Integer",
  "nonCompliantCount": "Integer",
  "notApplicableCount": "Integer",
  "remediatedCount": "Integer"
}
```

