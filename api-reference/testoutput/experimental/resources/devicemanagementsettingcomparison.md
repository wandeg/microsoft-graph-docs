---
title: "deviceManagementSettingComparison resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingComparison resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|comparisonResult|Enumeration|Setting comparison result. Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.|
|currentValueJson|String|JSON representation of current intent (or) template setting's value|
|definitionId|String|The ID of the setting definition for this instance|
|displayName|String|The setting's display name|
|id|String|The setting ID|
|newValueJson|String|JSON representation of new template setting's value|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```

