---
title: "outOfBoxExperienceSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# outOfBoxExperienceSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceUsageType|windowsDeviceUsageType|**TODO: Add Description**. Possible values are: `singleUser`, `shared`.|
|hideEscapeLink|Boolean|**TODO: Add Description**|
|hideEULA|Boolean|**TODO: Add Description**|
|hidePrivacySettings|Boolean|**TODO: Add Description**|
|skipKeyboardSelectionPage|Boolean|**TODO: Add Description**|
|userType|windowsUserType|**TODO: Add Description**. Possible values are: `administrator`, `standard`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": "Boolean",
  "hideEULA": "Boolean",
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": "Boolean",
  "hideEscapeLink": "Boolean"
}
```

