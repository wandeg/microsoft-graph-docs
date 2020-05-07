---
title: "dlpEvaluationWindowsDevicesInput resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# dlpEvaluationWindowsDevicesInput resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [dlpEvaluationInput](../resources/dlpevaluationinput.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessScope|accessScope|**TODO: Add Description** Inherited from [dlpEvaluationInput](../resources/dlpevaluationinput.md). Possible values are: `inOrganization`, `notInOrganization`.|
|contentProperties|[contentProperties](../resources/contentproperties.md)|**TODO: Add Description**|
|currentLabel|[currentLabel](../resources/currentlabel.md)|**TODO: Add Description** Inherited from [dlpEvaluationInput](../resources/dlpevaluationinput.md)|
|discoveredSensitiveTypes|[discoveredSensitiveType](../resources/discoveredsensitivetype.md) collection|**TODO: Add Description** Inherited from [dlpEvaluationInput](../resources/dlpevaluationinput.md)|
|sharedBy|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dlpEvaluationWindowsDevicesInput"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dlpEvaluationWindowsDevicesInput",
  "discoveredSensitiveTypes": [
    {
      "@odata.type": "microsoft.graph.discoveredSensitiveType"
    }
  ],
  "currentLabel": {
    "@odata.type": "microsoft.graph.currentLabel"
  },
  "accessScope": "String",
  "contentProperties": {
    "@odata.type": "microsoft.graph.contentProperties"
  },
  "sharedBy": "String"
}
```

