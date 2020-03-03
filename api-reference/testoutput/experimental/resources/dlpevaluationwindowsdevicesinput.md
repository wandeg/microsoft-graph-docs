---
title: "dlpEvaluationWindowsDevicesInput resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dlpEvaluationWindowsDevicesInput resource type


Namespace: microsoft.graph




Inherits from [dlpEvaluationInput](../resources/dlpevaluationinput.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessScope|Enumeration| Inherited from [dlpEvaluationInput](../resources/dlpevaluationinput.md). Possible values are: `inOrganization`, `notInOrganization`.|
|contentProperties|[contentProperties](../resources/contentproperties.md)||
|currentLabel|[currentLabel](../resources/currentlabel.md)| Inherited from [dlpEvaluationInput](../resources/dlpevaluationinput.md)|
|discoveredSensitiveTypes|[discoveredSensitiveType](../resources/discoveredsensitivetype.md) collection| Inherited from [dlpEvaluationInput](../resources/dlpevaluationinput.md)|
|sharedBy|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.discoveredSensitiveType",
      "id": "Guid",
      "count": 1024,
      "confidence": 1024
    }
  ],
  "currentLabel": {
    "@odata.type": "microsoft.graph.currentLabel",
    "id": "String",
    "applicationMode": "String"
  },
  "accessScope": "String",
  "contentProperties": {
    "@odata.type": "microsoft.graph.contentProperties",
    "extensions": [
      "String"
    ],
    "metadata": {
      "@odata.type": "microsoft.graph.contentMetadata"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "lastModifiedBy": "String"
  },
  "sharedBy": "String"
}
```

