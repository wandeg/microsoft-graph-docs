---
title: "deviceHealthScriptIntegerParameter resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptIntegerParameter resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deviceHealthScriptParameter](../resources/devicehealthscriptparameter.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applyDefaultValueWhenNotAssigned|Boolean|**TODO: Add Description** Inherited from [deviceHealthScriptParameter](../resources/intune-devicehealthscriptparameter.md)|
|defaultValue|Int32|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [deviceHealthScriptParameter](../resources/intune-devicehealthscriptparameter.md)|
|isRequired|Boolean|**TODO: Add Description** Inherited from [deviceHealthScriptParameter](../resources/intune-devicehealthscriptparameter.md)|
|name|String|**TODO: Add Description** Inherited from [deviceHealthScriptParameter](../resources/intune-devicehealthscriptparameter.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptIntegerParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptIntegerParameter",
  "name": "String",
  "description": "String",
  "isRequired": "Boolean",
  "applyDefaultValueWhenNotAssigned": "Boolean",
  "defaultValue": "Integer"
}
```

